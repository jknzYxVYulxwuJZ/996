#### 出售前触发

`beforesellqiugou`

| 参数     | 类型      | 空   | 默认 | 注释                 |
| :------- | :-------- | :--- | :--- | :------------------- |
| actor    | `object`  | 否   |      | 玩家对象             |
| itemName | `string`  | 否   |      | 出售物品名称         |
| itemIdx  | `integer` | 否   |      | 出售物品idx          |
| needNum  | `integer` | 否   |      | 出售的物品数量       |
| price    | `integer` | 否   |      | 出售的货币金额(总值) |
| result   | `bool`    | 否   |      | 是否允许本次出售     |
```lua
---出售前触发
---@param actor userdata 玩家对象
---@param itemName string 出售物品名称
---@param itemidx integer 出售物品idx
---@param num integer 出售的物品数量
---@param price integer 出售的货币金额(总值)
---@return boolean 是否允许本次出售
function beforesellqiugou(actor,itemName,itemidx,num,price,...)
    release_print("出售前触发",getbaseinfo(actor,1),itemidx,num,price,...)
    if getbaseinfo(actor,6) < 50 then
        messagebox(actor,"角色等级小于50级,无法出售道具~")
        return false
    end
    return true
end
```

