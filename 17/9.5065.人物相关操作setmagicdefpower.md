### 增加技能防御力
`setmagicdefpower`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |---|------      |
|play     |`object`    |否   |    |   玩家对象 |
|skillname     |`string`    |否   |    |  技能名称 |
|value     | `integer`    |否   |    |  抵消威力值 |
|type     | `integer`    |否   |    |  计算方式(0按点数计算,1按百分比计算) |
```lua
    setmagicdefpower(play,"雷电术",500,0)
```

