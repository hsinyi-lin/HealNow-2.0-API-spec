###### tags: `opendata`


# 新增某一類型某篇的opendata收藏 "POST"

> http://127.0.0.1:5000/opendatas/save_class/3/2
> 增加闢謠(3)的編號2收藏

## 回傳
| 欄位   | 中文 | 資料型態 |
| ------ | ---- | -------- |
| status | 狀態 | bool     |
| msg    | 訊息 | str      |


## 類型編號
* 編號1：藥品
* 編號2：食藥新聞
* 編號3：闢謠

## 範例

```json=
{
    "status": true,
    "msg": "成功"
}
```
