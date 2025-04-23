### 设置装备的元素属性

`setnewitemvalue`

| 参数    | 类型      | 空   | 默认                | 注释                     |
| :------ | :-------- | :--- | :------------------ | :----------------------- |
| play    | `object`  | 否   |                     | 玩家对象                 |
| itemPos | `integer` | 否   |                     | 装备位置(-2操作物品对象) |
| iAttr   | `integer` | 否   |                     | 属性                     |
| sFlag   | `string`  | 否   |                     | 比较符(=+-)              |
| iValue  | `integer` | 否   |                     | 数值(1-100)，百分比      |
| item    | `object`  | 否   | 引擎64_23.08.30新增 | 物品对象                 |
```lua
--根据装备位设置元素属性
setnewitemvalue(actor,1,1,"+",1)

--根据物品对象设置元素属性
setnewitemvalue(actor,-2,1,"+",100,itemobj)
```

