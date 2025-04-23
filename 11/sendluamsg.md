### 发送消息
`sendluamsg`

&gt; sMsg消息体最大长度16000字节

| 参数   | 类型      | 空   | 默认 | 注释     |
| :----- | :-------- | :--- | :--- | :------- |
| self   | `object`  | 否   |      | 玩家对象 |
| msgid  | `integer` | 否   |      | 消息ID   |
| param1 | `integer` | 是   |      | 参数1    |
| param2 | `integer` | 是   |      | 参数2    |
| param3 | `integer` | 是   |      | 参数3    |
| sMsg   | `string`  | 是   |      | 消息体   |

```lua
function handlerequest(self, msgid, n1, n2, n3, sMsg)
    if (msgid == 10) then
        release_print("收到10号消息")
    else
        sendluamsg(self, msgid, n1, n2, n3, sMsg)
    end
end
```

