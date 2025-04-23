### 获取自定义变量

`getguildvar`

| 参数    | 类型               | 空   | 默认 | 注释     |
| :------ | :----------------- | :--- | :--- | :------- |
| guild   | `object`           | 否   |      | 行会对象 |
| varName | `string`           | 否   |      | 变量名   |
| result  | `string`/`integer` |      |      | 变量值   |

```lua
function main(actor) 
    guild = getmyguild(actor)
    iniguildvar(guild, "integer", "N变量1")
    setguildvar(guild, "N变量1", 997)
    say(self, "自定义变量 N变量1="..getguildvar(guild, "N变量1"))
end
```
```lua
function main(actor) 
    guild = getmyguild(actor)
    iniguildvar(guild, "string", "S变量1|S变量2")
    setguildvar(guild, "S变量1", "引擎", 1)
    say(self, "自定义变量 S变量1="..getguildvar(guild, "S变量1"))
end
```

------------

## 变量操作

