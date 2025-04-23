### 回收触发

`recycling`

| 参数     | 类型      | 空   | 默认 | 注释       |
| :------- | :-------- | :--- | :--- | :--------- |
| actor    | `object`  | 否   |      | 玩家对象 |

```lua
function recycling(actor, ...)
    release_print("======================")
    release_print("recycling", getbaseinfo(actor, 1), ...)
    release_print("回收输出常量", getconst(actor, "<$RECYITEMS>"))
    release_print("回收总数常量", getconst(actor, "<$RECYITEMSCNT>"))
    release_print("回收获得总物品", getconst(actor, "<$TOTALRECYITEMS>"))
end
```
------------

## 接口

