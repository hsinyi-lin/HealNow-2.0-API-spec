###### tags: `auth`


# 註冊[POST]

> http://127.0.0.1:5000/auth/register

## 輸入
| 欄位     | 中文 | 資料型態 |
| -------- | ---- | -------- |
| email    | 信箱 | str      |
| password | 密碼 | str      |
| username | 名稱 | str      |
| gender   | 性別 | char     |


## 回傳
| 欄位         | 中文 | 資料型態 |
| ------------ | ---- | -------- |
| status       | 狀態 | bool     |
| msg          | 訊息 | str      |


## 範例
```json=
{
    "email":"11136004@ntub.edu.tw",
    "password": "12345",
    "username": "hsinyi",
    "gender": "F"
}
```


```json=
{
    "status": true,
    "msg": "成功"
}
```

## 注意
* gender僅有 "F" 或 "M"，F為女、M為男
