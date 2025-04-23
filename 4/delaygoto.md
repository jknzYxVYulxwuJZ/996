### 延时跳转
`delaygoto`

| 参数 | 类型      | 空   | 默认 | 注释                                          |
| :--- | :-------- | :--- | :--- | :-------------------------------------------- |
| play | `object`  | 否   |      | 玩家对象                                      |
| time | `integer` | 否   |      | 时间(毫秒)                                    |
| func | `string`  | 否   |      | 触发函数                                      |
| del  | `integer` | 否   |      | 换地图是否删除此延时(0或为空时=不删除 1=删除) |

```lua
    delaygoto(actor,1000,"test_jump,ceshi,44",0)

    --QFunction-0.lua
    function test_jump(actor,...)
        release_print(getbaseinfo(actor,1),...)
    end
```

