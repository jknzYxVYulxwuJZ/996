### 获取角色所有buff

`getallbuffid`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|player       |`object`        |否   |    |   玩家对象    |
|result |`table`       |是   |    |   buff列表    |
```lua
    local list_buff = getallbuffid(actor)
    for i, buffid in ipairs(list_buff) do
        release_print("buff",i,buffid)
    end
```

