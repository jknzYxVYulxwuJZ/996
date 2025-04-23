### 跨服通知触发本服QF

`kfbackcall`

| 参数   | 类型      | 空   | 默认 | 注释                                                                 |
| :----- | :-------- | :--- | :--- | :------------------------------------------------------------------- |
| id     | `integer` | 否   |      | 消息id（1-99）                                                       |
| userid | `string`  | 否   |      | 玩家userid<br />填`"0"`则是以系统对象发送通知,通知所有连接跨服的服务器 |
| parama | `string`  | 否   |      | 传递的字符串1(字符串)                                                |
| paramb | `string`  | 否   |      | 传递的字符串2(字符串)                                                |
```lua
    local userID = getbaseinfo(actor, 2)
    kfbackcall(22,userID,"跨服发送1","跨服发送2")   --玩家对象发送
    -- kfbackcall(22,"0","跨服发送3","跨服发送4")        --系统对象发送

    --跨服通知触发本服QF
    function kfsyscall22(actor,arg1,arg2)
        local role_name = getbaseinfo(actor, 1)
        release_print("跨服通知触发本服QF",role_name,arg1,arg2)
    end

```

<br />

