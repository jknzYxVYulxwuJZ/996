### 刷怪
`genmon`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|mapid     |`string`      |否   |    |   地图id |
|x     |`integer`      |否   |    |  坐标X |
|y     |`integer`      |否   |    |   坐标Y |
|monname     |`string`      |否   |    |   怪物名称 |
|range     |`integer`      |否   |    |   范围 |
|count     |`integer`      |否   |    |   数量 |
|color     |`integer`      |否   |    |   颜色(0~255) |
|result     |`table`      |否   |    |   返回怪物列表 |
```lua
    genmon(0,289,613,"稻草人",10,10)
```

