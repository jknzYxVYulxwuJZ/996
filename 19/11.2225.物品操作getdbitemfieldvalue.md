### 获取物品原始各项数据库字段值参数

`getdbitemfieldvalue`

| 参数             | 类型               | 空   | 默认 | 注释            |
| :--------------- | :----------------- | :--- | :--- | :-------------- |
| itemIdx/itemName | `integer`/`string` | 否   |      | 物品ID/物品名称 |
| fieldName        | `string`           | 否   |      | 字段名          |

```lua
    local config = {
        {"Name", "1列"},
        {"StdMode", "2列"},
        {"Shape", "3列"},
        {"Weight", "4列"},
        {"Anicount", "5列"},
        {"Source", "6列"},
        -- {"Reserved", "7列"},      --接口无法获取,服务器不读取
        {"Looks", "8列"},
        {"DuraMax", "9列"},
        {"Attribute", "10列"},
        {"Need", "11列"},
        {"NeedLevel", "12列"},
        {"NeedLevelParam", "12列","NeedLevel#后的数据"},
        {"Price", "13列"},
        {"Color", "14列"},
        {"OverLap", "15列"},        --装备无法获取堆叠数量,固定返回值为0
        -- {"Suit", "16列"},        --当前引擎已取消16列
        {"Article", "17列"},
        {"Job", "18列"},
        {"effectParam", "19列"},
        -- {"Desc", "20列"},        --接口无法获取,服务器不读取
        -- {"pickset", "21列"},     --接口无法获取,服务器不读取
        -- {"guangzhu", "22列"},    --接口无法获取,服务器不读取
        -- {"auctionby", "23列"},   --接口无法获取,服务器不读取
        {"sEffect", "24列"},
        {"bEffect", "25列"},
        {"rizhi", "27列"},          --引擎2024.03.14修复无法获取问题
        {"zblmtkz", "28列"},        --引擎2024.03.14修复无法获取问题
        {"ITEMPAEAM1", "29列"},
        {"ITEMPAEAM2", "30列"},
        -- {"Comparison", "31列"},  --接口无法获取,服务器不读取
        {"suit", "32列"},           --32列的suitid更名为suit
        {"Insurance", "33列"},
        -- {"pickCondition", "34列"},--接口无法获取,服务器不读取
    }
    for _, v in ipairs(config) do
        release_print("对应item/equip表",v[2],v[1]..(v[3] or ""),getdbitemfieldvalue("20000元宝", v[1]))
    end
```

