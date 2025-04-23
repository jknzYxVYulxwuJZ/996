### 请求行会联盟前触发

`guildapplybefore`

| 参数      | 类型      | 空   | 默认 | 注释                              |
| :-------- | :-------- | :--- | :--- | :-------------------------------- |
| play      | `object`  | 否   |      | 发起请求玩家对象                  |
| guildName | `string`  | 否   |      | 行会名字                          |
| time      | `integer` | 否   |      | 结盟时长(小时)                    |
| moneyType | `integer` | 否   |      | 货币类型                          |
| moneyNum  | `integer` | 否   |      | 货币数量                          |
| result    | `bool`    | 是   |      | true=允许发起<br />false=不允许发起 |
```lua
function guildapplybefore(actor,guildName,time,moneyType,moneyNum)
    return true
end
```

