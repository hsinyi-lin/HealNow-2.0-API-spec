###### tags: `user`


# 編輯個人資料"PATCH"

> http://127.0.0.1:5000/user


## 輸入
| 欄位     | 中文       | 資料型態   |
| -------- | ---------- | ---------- |
| username | 使用者名稱 | bool       |
| gender   | 性別       | str        |
| photo    | 頭貼       | base64 str |

**在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態**


## 回傳
| 欄位   | 中文 | 資料型態 |
| ------ | ---- | -------- |
| status | 狀態 | bool     |
| msg    | 訊息 | str      |


## 範例

```json=
{
    "username": "hsin",
    "gender": "F",
    "photo": "/9j/4AAQSkZJRgABAQAAAQABA..."
}
```

```json=
{
    "status": true,
    "msg": "成功"
}
```

## 備註
* 為了避免base64過長而導致資料庫讀取過慢，請在前端先把圖片進行壓縮後，再轉成base64傳給後端。或許可參考"flutter_image_compress"壓縮套件。
* 不論是進行「頭貼」、「名稱」、「性別」更新，呼叫此API時，將「不進行更新」的資料也一同傳給後端。