###### tags: `comment`


# 取得單一回覆"GET"

> http://127.0.0.1:5000/comments/3
針對回覆編號 3

## 輸入

**在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態**


## 回傳
| 欄位   | 中文 | 資料型態 |
| ------ | ---- | -------- |
| status | 狀態 | bool     |
| msg    | 訊息 | str      |
| data    | 資訊 | object      |

### data 內容

| 欄位         | 中文         | 資料型態 |
| ------------ | ------------ | -------- |
| id           | 回覆編號     | int      |
| post_id      | 貼文編號     | int      |
| content      | 回覆內容     | str      |
| created_time | 回覆建立時間 | datetime |
| updated_time | 回覆更新時間 | datetime |


## 範例


```json=
{
    "status": true,
    "msg": "成功",
    "data": {
        "content": "去散散步!!",
        "created_time": "Mon, 11 Dec 2023 21:58:44 GMT",
        "id": 3,
        "post_id": 3,
        "updated_time": "Mon, 11 Dec 2023 22:04:27 GMT"
    }
}
```
