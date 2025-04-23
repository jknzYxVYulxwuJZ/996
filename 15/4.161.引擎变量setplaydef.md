### 设置玩家变量

`setplaydef`

| 参数    | 类型               | 空   | 默认 | 注释     |
| :------ | :----------------- | :--- | :--- | :------- |
| actor   | `object`           | 否   |      | 玩家对象 |
| varName | `string`           | 否   |      | 变量名   |
| value   | `string`/`integer` |      |      | 变量值   |

> **支持自定义临时变量**
 格式：1.自定义数字变量，以`N$`为头标志；
 2.自定义字符变量，以`S$`为头标志
 
```lua
  --玩家变量示例
    setplaydef(actor, "U1",1)
    say(actor, "玩家数字变量U1变量="..getplaydef(actor,"U1"))

  --临时玩家变量示例
    setplaydef(actor, "N$变量1",1)
    say(actor, "自定义数字变量N$变量1="..getplaydef(actor,"N$变量1"))
```

```lua
    [[lua获取TXT命令设置的高效率版键值对,仅作参考,可根据自身需求修改]]
    function getVarCache(actor,varName,key)
        local str = getplaydef(actor,varName)
        local result = {}
        for k, v in string.gmatch(str, "([^=]+)=([^,]+)") do
            k = k:gsub(",", "")
            result[k] = v
        end
        return result[tostring(key)] or ""
    end

    local value = getVarCache(actor,"T1",1)
```

