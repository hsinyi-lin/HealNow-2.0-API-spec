###### tags: `auth`


# 更改密碼"PATCH"

> http://127.0.0.1:5000/auth/change_password

## 輸入
| 欄位                          | 中文     | 資料型態 |
| ----------------------------- | -------- | -------- |
| is_login                      | 是否登入 | bool     |
| email(非登入狀態才補上此欄位) | 帳號     | str      |
| new_password                  | 新密碼   | str      |

**如果是登入狀態使用，需在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態，否則就不需要，但要補上email欄位**


## 回傳
| 欄位         | 中文 | 資料型態 |
| ------------ | ---- | -------- |
| status       | 狀態 | bool     |
| msg          | 訊息 | str      |

## 備註


## 範例
```json=

// 非登入狀態
{
    "is_login": false,
    "email": "11136004@ntub.edu.tw",
    "new_password": "1234567"
}

// 登入狀態
{
    "is_login": true,
    "new_password": "1234567"
}
```


```json=
{
    "status": true,
    "msg": "成功"
}
```
