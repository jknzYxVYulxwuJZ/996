### 获取背包物品列表

`getbagitems`

| 参数     | 类型      | 空   | 默认                | 注释                                     |
| :------- | :-------- | :--- | :------------------ | :--------------------------------------- |
| player   | `object`  | 否   |                     | 玩家对象                                 |
| itemName | `string`  | 否   | 引擎64_23.10.24新增 | 道具名字                                 |
| isbind   | `integer` | 否   | 引擎64_23.10.24新增 | 是否绑定<br />0=忽略<br />1=非绑定<br />2=绑定 |
| result   | `table`   | 是   |                     | 道具列表                                 |
```lua
    local items
    if sMsg == "1" then
        release_print("获取背包所有物品")
        items = getbagitems(actor)
    elseif sMsg == "2" then
        release_print("获取背包所有非绑定物品")
        items = getbagitems(actor,nil,1)
    elseif sMsg == "3" then
        release_print("获取背包所有绑定物品")
        items = getbagitems(actor,nil,2)
    elseif sMsg == "4" then
        release_print("获取背包非绑定木剑")
        items = getbagitems(actor,"木剑",1)
    elseif sMsg == "5" then
        release_print("获取背包绑定木剑")
        items = getbagitems(actor,"木剑",2)
    elseif sMsg == "6" then
        release_print("获取背包所有木剑")
        items = getbagitems(actor,"木剑")
    end
    if type(items) ~= "table" then return end
    for i, itemobj in pairs(items or {}) do
        local isBind = getiteminfo(actor,itemobj,6)
        local itemName = getiteminfo(actor,itemobj,7)
        release_print("item["..i.."]",itemName,isbind)
    end
```

------------

