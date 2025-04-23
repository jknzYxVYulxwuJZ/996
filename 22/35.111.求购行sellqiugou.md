#### 卖出成功触发

`sellqiugou`

| 参数     | 类型      | 空   | 默认 | 注释                 |
| :------- | :-------- | :--- | :--- | :------------------- |
| actor    | `object`  | 否   |      | 玩家对象             |
| itemName | `string`  | 否   |      | 卖出物品名称         |
| itemIdx  | `integer` | 否   |      | 卖出物品idx          |
| needNum  | `integer` | 否   |      | 卖出的物品数量       |
| price    | `integer` | 否   |      | 卖出的货币金额(总值) |
```lua
---卖出成功触发
---@param actor userdata 玩家对象
---@param itemName string 卖出物品名称
---@param itemidx integer 卖出物品idx
---@param num integer 卖出的物品数量
---@param price integer 卖出的货币金额(总值)
function sellqiugou(actor,itemName,itemidx,num,price,...)
    release_print("卖出成功触发",getbaseinfo(actor,1),itemidx,num,price,...)
end
```
