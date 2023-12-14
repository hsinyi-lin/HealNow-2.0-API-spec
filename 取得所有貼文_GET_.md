###### tags: `post`


# 取得所有貼文"GET"

> http://127.0.0.1:5000/posts


## 回傳
| 欄位         | 中文 | 資料型態 |
| ------------ | ---- | -------- |
| status       | 狀態 | bool     |
| msg          | 訊息 | str      |
| data          | 資料 | object      |


### data 內容
| 欄位         | 中文     | 資料型態 |
| ------------ | -------- | -------- |
| id           | 貼文編號 | int      |
| title        | 標題     | str      |
| content      | 內容     | str      |
| email        | 貼文者   | str      |
| created_time | 建立時間 | datetime |
| updated_time | 更新時間 | datetime |



## 範例

```json=
{
    "status": true,
    "msg": "成功",
    "data": [
        {
            "content": "去散散步",
            "created_time": "Mon, 11 Dec 2023 21:28:30 GMT",
            "email": "11136004@ntub.edu.tw",
            "id": 3,
            "title": "今天天氣不錯",
            "updated_time": "Mon, 11 Dec 2023 21:28:30 GMT"
        }
    ]
}
```
