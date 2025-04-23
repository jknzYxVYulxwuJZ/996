### 召唤宝宝
`recallmob`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|player     |`object`      |否   |    |玩家对象 |
|monName     |`string`      |否   |    |   怪物名称 |
|level     |`integer`      |否   |    |宝宝等级(最高为7) |
|time     |`integer`      |否   |    |叛变时间(分钟) |
|param1     |`integer`      |否   |    |预留(填0) |
|param2     |`integer`      |否   |    |预留(填0) |
|param3     |`integer`      |否   |    |设置大于0，检测时不计算该宝宝数量(仅M2控制的召唤数量) |
|result     |`object`      |否   |    |   宝宝对象 |
```lua
    local mon = recallmob(actor,"神兽",7,30,1)
    release_print("成功召唤",getbaseinfo(mon,1))
```

