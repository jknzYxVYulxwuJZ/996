### 获取人物所有称号

`newgettitlelist`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.03.14新增接口&lt;/font&gt;**

| 参数   | 类型     | 空   | 默认 | 注释         |
| :----- | :------- | :--- | :--- | :----------- |
| play   | `object` | 否   |      | 玩家对象     |
| result | `table`  | 否   |      | 返回称号列表<br />[称号id]=时间戳 |

```lua
    local titlelist = newgettitlelist(actor)
    for titleID, endTime in pairs(titlelist or {}) do
        local titleName = getstditeminfo(titleID,1)
        release_print("称号",titleName,titleID,os.date("%Y-%m-%d %H:%M:%S",endTime))
    end
```

