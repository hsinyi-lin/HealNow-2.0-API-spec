###### tags: `auth`


# 登入"POST"

> http://127.0.0.1:5000/auth/login

## 輸入
| 欄位     | 中文 | 資料型態 |
| -------- | ---- | -------- |
| email    | 信箱 | str      |
| password | 密碼 | str      |


## 回傳
| 欄位         | 中文 | 資料型態 |
| ------------ | ---- | -------- |
| status       | 狀態 | bool     |
| msg          | 訊息 | str      |
| access_token | 權杖 | str      |


## 範例
```json=
{
    "email":"11136004@ntub.edu.tw",
    "password": "1234567"
}
```


```json=
{
    "status": true,
    "msg": "成功",
    "access_token": "ejfipqjefpq..."
}
```
