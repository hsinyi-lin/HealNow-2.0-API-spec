###### tags: `post`


# 新增貼文"POST"

> http://127.0.0.1:5000/posts/3
編號 3 貼文

## 輸入
| 欄位    | 中文 | 資料型態 |
| ------- | ---- | -------- |
| title   | 標題 | str      |
| content | 內容 | str      |

**在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態**


## 回傳
| 欄位   | 中文 | 資料型態 |
| ------ | ---- | -------- |
| status | 狀態 | bool     |
| msg    | 訊息 | str      |


## 範例

```json=
{
    "title": "今天天氣不錯!",
    "content": "去散散步~"
}
```

```json=
{
    "status": true,
    "msg": "成功"
}
```
