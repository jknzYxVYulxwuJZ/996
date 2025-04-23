### 设定地图定时器
`setenvirontimer`

| 参数   | 类型      | 空   | 默认 | 注释                             |
| :----- | :-------- | :--- | :--- | :------------------------------- |
| MapId  | `string`  | 否   |      | 地图ID                           |
| Idx    | `integer` | 否   |      | 计时器ID                         |
| second | `integer` | 否   |      | 时长（秒）                       |
| func   | `string`  | 否   |      | 触发跳转的函数(多参数用逗号分割) |

```lua
 setenvirontimer(0,1,10,"@test_jump,aaa,bbb")

[[跳转函数参数1为系统对象,传递的参数从参数2开始]]
function test_jump(sysobj,...)
    release_print(...)
end
```

