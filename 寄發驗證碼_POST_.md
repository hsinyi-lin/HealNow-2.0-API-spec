###### tags: `auth`


# 寄發驗證碼"POST"

> http://127.0.0.1:5000/auth/send_verification

## 輸入
| 欄位     | 中文 | 資料型態 |
| -------- | ---- | -------- |
| email    | 信箱 | str      |


## 回傳
| 欄位         | 中文 | 資料型態 |
| ------------ | ---- | -------- |
| status       | 狀態 | bool     |
| msg          | 訊息 | str      |


## 範例
```json=
{
    "email": "11136004@ntub.edu.tw"
}
```


```json=
{
    "status": true,
    "msg": "成功"
}
```
