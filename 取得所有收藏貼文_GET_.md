###### tags: `save`


# 取得所有收藏貼文"GET"

> http://127.0.0.1:5000/saves

## 輸入

**在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態**


## 回傳
| 欄位   | 中文 | 資料型態 |
| ------ | ---- | -------- |
| status | 狀態 | bool     |
| msg    | 訊息 | str      |
| data   | 資料 | object   |

### data內容
| 欄位         | 中文     | 資料型態 |
| ------------ | -------- | -------- |
| post_id      | 貼文編號 | int      |
| email        | 發文者   | str      |
| username        | 發文者名稱   | str      |
| title        | 標題     | str      |
| content      | 內容     | str      |
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
            "username": "hsin",
            "post_id": 10,
            "title": "今天天氣不錯",
            "updated_time": "Mon, 11 Dec 2023 21:28:30 GMT"
        },
        {
            "content": "去散散步",
            "created_time": "Mon, 11 Dec 2023 21:28:30 GMT",
            "email": "11136004@ntub.edu.tw",
            "username": "hsin",
            "post_id": 11,
            "title": "今天天氣不錯",
            "updated_time": "Mon, 11 Dec 2023 21:28:30 GMT"
        }
    ]
}
```

## 備註
如果要再取得單一收藏貼文內容，自行根據貼文ID呼叫該貼文的API