### 给NPC注册Lua消息
`regnpcmsg`

| 参数     | 类型  | 空   | 默认 | 注释                       |
| :------- | :---- | :--- | ---- | -------------------------- |
| msgId    | `int` | 否   |      | 消息ID                     |
| NPCIndex | `int` | 否   |      | NPC索引（NPC配置表中的ID） |

```
给NPC注册LUA消息后，当服务器接收到Lua消息，如果有对应的NPC且玩家在NPC有效区域（同地图且在NPC附近）内，则激活NPC脚本内容（相当于点击了NPC）
```

