###### tags: `auth`


# 更改密碼"PATCH"

> http://127.0.0.1:5000/auth/change_password

## 輸入
| 欄位         | 中文   | 資料型態 |
| ------------ | ------ | -------- |
| new_password | 新密碼 | str      |

**在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態**


## 回傳
| 欄位         | 中文 | 資料型態 |
| ------------ | ---- | -------- |
| status       | 狀態 | bool     |
| msg          | 訊息 | str      |


## 範例
```json=
{
    "new_password": "1234567"
}
```


```json=
{
    "status": true,
    "msg": "成功"
}
```
