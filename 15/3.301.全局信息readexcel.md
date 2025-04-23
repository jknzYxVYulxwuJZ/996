### 读取表格

`readexcel`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.03.14新增接口&lt;/font&gt;**

| 参数   | 类型     | 空   | 默认 | 注释                 |
| :----- | :------- | :--- | :--- | :------------------- |
| path   | `string` | 否   |      | 表格路径             |
| result | `table`  | 否   |      | 返回表格所有数据内容 |

```lua
    local readPath = "../DATA/cfg_npclist.xls"
    local config = readexcel(readPath)
    release_print("readexcel",readPath,type(config))
    for i, cfg in ipairs(config or {}) do
        release_print("============================")
        -- if i &gt; 10 then return end
        if type(cfg) == "table" then
            for j, value in ipairs(cfg) do
                release_print("config",i,j,value)
            end
        end
    end
```

------------

