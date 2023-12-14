###### tags: `save`


# 刪除收藏貼文"DELETE"

> http://127.0.0.1:5000/saves/3
貼文編號 3

## 輸入

**在 Headers 加上 Authorization，內容再以 Bearer + token 以表示使用者登入狀態**


## 回傳
| 欄位   | 中文 | 資料型態 |
| ------ | ---- | -------- |
| status | 狀態 | bool     |
| msg    | 訊息 | str      |


## 範例

```json=
{
    "status": true,
    "msg": "成功"
}
```
