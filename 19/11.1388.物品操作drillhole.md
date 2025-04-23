### 装备开孔
`drillhole`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|item     |`object`        |否   |    |  装备对象   |
|holejson  |`string`       |否   |    |  开孔相关，json字符串，支持0~9共10个孔    |
```lua
    local config = {}
    for i = 0, 9 do
        config["hole"..i] = 1 -- 0-不开孔，1-开孔
    end
    drillhole(actor,itemobj,tbl2json(config))
    release_print("开孔信息1",getdrillhole(actor,itemobj))

    -- * 不要求所有空数据都传送，允许只传指定孔的字符串，例如：
    local config = {}
    config.hole0 = 1 -- 0-不开孔，1-开孔
    drillhole(actor,itemobj,tbl2json(config))
    release_print("开孔信息2",getdrillhole(actor,itemobj))
```

