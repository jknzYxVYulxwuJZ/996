### 初始化自定义变量

`iniplayvar`

| 参数      | 类型     | 空   | 默认 | 注释                         |
| :-------- | :------- | :--- | :--- | :--------------------------- |
| actor     | `object` | 否   |      | 玩家对象                     |
| varType   | `string` | 否   |      | 变量类型(integer/string)     |
| varScope  | `string` | 否   |      | 变量范围(HUMAN/GUILD/NATION) |
| varName   | `string` | 否   |      | 变量名                       |

```lua
-- 角色登陆触发
function login(actor)
    iniplayvar(actor, "integer", "HUMAN", "玩家变量_1")
    iniplayvar(actor, "string", "HUMAN", "玩家变量_2")
end
```

