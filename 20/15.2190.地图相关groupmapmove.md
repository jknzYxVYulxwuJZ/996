### 编组地图传送
`groupmapmove`

| 参数  | 类型      | 空   | 默认 | 注释                                                       |
| :---- | :-------- | :--- | :--- | :--------------------------------------------------------- |
| play  | `object`  | 否   |      | 玩家对象                                                   |
| MapId | `string`  | 否   |      | 地图ID                                                     |
| x     | `integer` | 否   |      | x坐标                                                      |
| y     | `integer` | 否   |      | y坐标                                                      |
| level | `integer` | 否   |      | 可以传送最低等级(可以为空，为空时不检测队员的等级直接传送) |
| value | `integer` | 否   |      | 传送范围。（以队长为中心传送队友，0为不需要范围）          |
| obj   | `object`  | 是   |      | 触发字段(可以为空)                                         |
```lua
    groupmapmove(actor,3,333,333,nil,0,"testjump")
    function testjump(actor)
        release_print("testjump",getbaseinfo(actor,1))
    end
```

