#### 求购上架成功触发

`addqiugou`

| 参数     | 类型      | 空   | 默认 | 注释                 |
| :------- | :-------- | :--- | :--- | :------------------- |
| actor    | `object`  | 否   |      | 玩家对象             |
| itemName | `string`  | 否   |      | 求购物品名称         |
| itemIdx  | `integer` | 否   |      | 求购物品idx          |
| needNum  | `integer` | 否   |      | 求购的物品数量       |
| price    | `integer` | 否   |      | 求购的货币金额(总值) |
| result   | `bool`    | 否   |      | 是否允许本次求购     |
```lua
---求购上架成功触发
---@param actor userdata 玩家对象
---@param itemName string 求购物品名称
---@param itemidx integer 求购物品idx
---@param needNum integer 求购的物品数量
---@param price integer 求购的货币金额(总值)
---@return boolean 是否允许本次求购
function addqiugou(actor,itemName,itemidx,needNum,price,...)
    release_print("求购上架成功触发",getbaseinfo(actor,1),itemidx,needNum,price,...)
end
```

