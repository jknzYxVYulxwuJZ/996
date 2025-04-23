### 掌门踢出行会成员前触发

`guildchiefdelmember`

| 参数   | 类型     | 空   | 默认 | 注释                          |
| :----- | :------- | :--- | :--- | :---------------------------- |
| play   | `object` | 否   |      | 玩家对象                      |
| userID | `string` | 否   |      | 被踢玩家userID                |
| result | `bool`   | 是   |      | true=允许踢<br />false=不允许踢 |
```lua
function guildchiefdelmember(actor,userID)
    return true
end

```

## 接口

