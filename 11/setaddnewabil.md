### 装备批量增加附加属性

`setaddnewabil`

| 参数    | 类型      | 空   | 默认 | 注释                     |
| :------ | :-------- | :--- | :--- | :----------------------- |
| play    | `object`  | 否   |      | 玩家对象                 |
| where   | `integer` | 否   |      | 装备位置(-2操作物品对象) |
| opt     | `string`  | 否   |      | 运算符(+,-,=)            |
| attrStr | `string`  | 否   |      | 属性组                   |
| item    | `object`  | 否   |      | 物品对象                 |
```lua
--根据装备位加属性
setaddnewabil(actor,1,"+","3#3#2|3#4#10|3#4#2|3#5#10|3#23#2|3#74#10")

--根据物品对象加属性
setaddnewabil(actor,-2,"+","3#3#2|3#4#10|3#4#2|3#5#10|3#23#2|3#74#10",itemobj)
```

