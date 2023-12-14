###### tags: `mood`


# 取得所有心情紀錄"GET"

> http://127.0.0.1:5000/moods

## 輸入

**在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態**


## 回傳
| 欄位   | 中文 | 資料型態 |
| ------ | ---- | -------- |
| status | 狀態 | bool     |
| msg    | 訊息 | str      |
| data   | 資料 | object   |

### data內容
| 欄位         | 中文         | 資料型態 |
| ------------ | ------------ | -------- |
| id           | 心情紀錄編號 | int      |
| email        | 本人         | str      |
| content      | 內容         | str      |
| ai_reply     | AI回覆       | str      |
| created_time | 建立時間     | datetime |


## 範例

```json=
{    
    "success": true,
    "msg": "成功",
    "data": [
        {
            "ai_reply": "每一場雨終究會有結束的時候，對於未來的陽光，你需要保持耐心和堅持，相信明天會更好。",
            "content": "今天下了一整天的雨，好煩躁",
            "created_time": "Mon, 11 Dec 2023 23:54:15 GMT",
            "email": "11136004@ntub.edu.tw",
            "id": 3
        },
        {
            "ai_reply": "不要害怕迎接新的挑戰，因為你已經有足夠的力量去克服困難。",
            "content": "今天天氣真好",
            "created_time": "Mon, 11 Dec 2023 23:54:15 GMT",
            "email": "11136004@ntub.edu.tw",
            "id": 4
        }
    ]
}
```
