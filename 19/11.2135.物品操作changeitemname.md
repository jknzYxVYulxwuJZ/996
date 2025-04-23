### 修改物品/装备名称

`changeitemname`

| 参数     | 类型      | 空   | 默认                | 注释                     |
| :------- | :-------- | :--- | :------------------ | :----------------------- |
| play     | `object`  | 否   |                     | 玩家对象                 |
| itemPos  | `integer` | 否   |                     | 装备位置(-2操作物品对象) |
| itemName | `string`  | 否   |                     | 装备名字                 |
| item     | `object`  | 否   | 引擎64_23.08.30新增 | 物品对象                 |
```lua
--根据装备位改名
changeitemname(actor,1,"装备改名1")

--根据物品对象改名
changeitemname(actor,-2,"装备改名2",itemobj)

--怪物物品掉落回调接口
function mondropitemex(actor, itemobj, monobj, x, y)
    [[引擎64_23.10.24支持刷新地面物品的名字,之前引擎需要调用TXT命令]]
    changeitemname(actor,-2,"测试道具_lua22",itemobj)
    changeitemnamecolor(actor,itemobj,199)
    refreshitem(actor,itemobj)
    
    [[之前的引擎需要调用TXT命令]]
    -- callscriptex(actor,"LINKPICKUPITEM")
    -- callscriptex(actor,"ChangeItemName",-1,"测试道具_txt2")
    -- callscriptex(actor,"changeitemnamecolor",-1,200)
    -- callscriptex(actor,"SENDUPGRADEITEM")
end
```

