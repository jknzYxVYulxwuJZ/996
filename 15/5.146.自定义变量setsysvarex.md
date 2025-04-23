### 设置自定义变量

`setsysvarex`

| 参数    | 类型               | 空   | 默认 | 注释                                 |
| :------ | :----------------- | :--- | :--- | :----------------------------------- |
| varName | `string`           | 否   |      | 变量名                               |
| value   | `string`/`integer` | 否   |      | 变量值                               |
| isSave  | `integer`          | 是   | 0    | 是否保存数据库<br>0=不存储<br>1=存储 |

```lua
    --系统变量示例
    local varName = "系统自定义变量_1"
    inisysvar("integer",varName,0)
    setsysvarex(varName,996,1)
    release_print("系统自定义变量[integer]",varName,getsysvarex(varName))

    local varName = "系统自定义变量_2"
    inisysvar("string",varName,0)
    setsysvarex(varName,"996abc",1)
    release_print("系统自定义变量[string]",varName,getsysvarex(varName))
```

------------

## 玩家自定义变量

> **玩家自定义变量需要初始化后才能使用**
> **玩家每次登陆都需要初始化**
> **一个变量名不允许初始化两种变量类型**

