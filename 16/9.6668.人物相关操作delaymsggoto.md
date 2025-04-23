### 延时消息跳转
`delaymsggoto`

| 参数 | 类型      | 空   | 默认 | 注释       |
| :--- | :-------- | :--- | :--- | :--------- |
| play | `object`  | 否   |      | 玩家对象   |
| time | `integer` | 否   |      | 时间(毫秒) |
| func | `string`  | 否   |      | 触发函数   |
通过消息机制实现延时跳转，允许触发函数内嵌跳转，实现多次跳转，需要传递参数，将参数与函数名使用“,”连接。
本延时跳转不支持删除。
```lua
    delaymsggoto(actor, 2000, "@test_jump,ceshi,55")

    --QFunction-0.lua
    function test_jump(actor,...)
        release_print(getbaseinfo(actor,1),...)
    end
```

------------

