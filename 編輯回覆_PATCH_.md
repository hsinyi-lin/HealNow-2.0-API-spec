###### tags: `comment`


# 編輯回覆"PATCH"

> http://127.0.0.1:5000/comments/10
針對回覆編號 10 

## 輸入
| 欄位    | 中文 | 資料型態 |
| ------- | ---- | -------- |
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
    "content": "去散散步~"
}
```

```json=
{
    "status": true,
    "msg": "成功"
}
```
