### 给物品

 `giveitem`

| 参数     | 类型      | 空   | 默认                | 注释                                                                                                                                   |
| :------- | :-------- | :--- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------------- |
| play     | `object`  | 否   |                     | 玩家对象                                                                                                                               |
| itemname | `string`  | 否   |                     | 物品名称                                                                                                                               |
| qty      | `integer` | 是   | 1                   | 数量                                                                                                                                   |
| bind     | `integer` | 是   | 0                   | 物品规则                                                                                                                               |
| desc     | `string`  | 是   | 引擎64_24.05.23新增 | 描述                                                                                                                                   |
| result   | `object`  | 否   |                     | 返回值(最后一个物品对象)，不建议使用在叠加物品，一次性给多个物品的情况，此物品在添加背包触发后，注意可能被回收的情况 生成失败则返回nil |

```lua
    local item = giveitem(actor,"木剑",1,128,"测试")
```

