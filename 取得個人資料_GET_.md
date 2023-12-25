###### tags: `user`


# 取得個人資料"GET"

> http://127.0.0.1:5000/user


## 輸入

**在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態**


## 回傳
| 欄位   | 中文 | 資料型態 |
| ------ | ---- | -------- |
| status | 狀態 | bool     |
| msg    | 訊息 | str      |
| data    | 資料 | object      |


### data 內容

| 欄位         | 中文         | 資料型態   |
| ------------ | ------------ | ---------- |
| username     | 名稱         | str        |
| email        | 信箱         | str        |
| gender       | 性別         | char       |
| password     | 密碼         | str        |
| photo        | 頭貼         | base64 str |
| created_time | 資訊建立時間 | datetime   |
| updated_time | 資訊更新時間 | datetime   |


## 範例

```json=
{
    "status": true,
    "msg": "成功",
    "data": {
        "username": "hsin",
        "email": "11136004@ntub.edu.tw",
        "gender": "F",
        "password": "hash password...",
        "photo": "base64 string...",
        "created_time": "Mon, 11 Dec 2023 17:51:34 GMT",
        "updated_time": "Mon, 25 Dec 2023 18:42:32 GMT"
    }
}
```

## 備註
* 為了避免base64過長而導致資料庫讀取過慢，請在前端先把圖片進行壓縮後，再轉成base64傳給後端。或許可參考"flutter_image_compress"壓縮套件。
* 不論是進行「頭貼」、「名稱」、「性別」更新，呼叫此API時，將「不進行更新」的資料也一同傳給後端。