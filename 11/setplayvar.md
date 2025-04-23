### 设置自定义变量

`setplayvar`

| 参数     | 类型               | 空   | 默认 | 注释                                 |
| :------- | :----------------- | :--- | :--- | :----------------------------------- |
| actor    | `object`           | 否   |      | 玩家对象                             |
| varScope | `string`           | 否   |      | 变量范围(HUMAN/GUILD/NATION)         |
| varName  | `string`           | 否   |      | 变量名                               |
| value    | `string`/`integer` | 否   |      | 变量值                               |
| isSave   | `integer`          | 是   | 0    | 是否保存数据库<br>0=不存储<br>1=存储 |

```lua
    --系统变量示例
    local varName = "玩家自定义变量_1"
    iniplayvar(actor, "integer", "HUMAN", varName)
    setplayvar(actor,"HUMAN",varName,996,1)
    release_print("玩家自定义变量[integer]",varName,getplayvar(actor,varName))

    local varName = "玩家自定义变量_2"
    iniplayvar("string",varName,0)
    setplayvar(actor,"HUMAN",varNamem,"996abc",1)
    release_print("玩家自定义变量[string]",varName,getplayvar(actor,varName))
```

------------

## 行会自定义变量（由行会对象操作自定义变量）

