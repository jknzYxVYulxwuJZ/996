### 在地图上生成掉落物品

`gendropitem`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数   | 类型      | 空   | 默认               | 注释                                                 |
| :----- | :-------- | :--- | :----------------- | :--------------------------------------------------- |
| mapid  | `string`  | 否   |                    | 地图id                                               |
| actor  | `object`  | 是   |                    | 归属对象<br />填nil则无归属<br />且拾取cd时间会被设置为0 |
| X      | `integer` | 否   |                    | x坐标                                                |
| Y      | `integer` | 否   |                    | y坐标                                                |
| json   | `string`  | 否   |                    | 掉落json                                             |
| data   | `string`  | 否   |                    | 物品来源(参考设置物品来源)                           |
| range  | `integer` | 是   | 引擎64_24.0807新增 | 范围                                                 |
| result | `table`   | 否   |                    | 物品makeindex列表                                    |
```lua
    local items = {
        ["木剑"] = 100,
        ["金币"] = 996,
    }
    local data = {
        ["map"] =  mapID, --地图号
        ["source"] =  5,  --来源：1-GM生成，2-NPC，3-商城，4-NPC商店, 5-怪物掉落，6-系统给["与，7-挖矿，8-批量生成，9-宝箱
        ["mon"] = "白野猪",  --掉落的怪物
        ["player"] = "玩家人物名称qf",
        -- ["time"]=os.date("%Y-%m-%d %H:%M:%S", os.time()),  --掉落或生成的时间，为空时，设置为系统时间
    }
    local itemList = gendropitem(mapID,actor,x,y,tbl2json(items),tbl2json(data))
    -- local itemList = gendropitem(mapID,nil,x,y,tbl2json(items),tbl2json(data))
```

