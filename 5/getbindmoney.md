### 获取人物通用货币数量(多货币计算)
`getbindmoney`

| 参数      | 类型      | 空   | 默认 | 注释       |
| :-------- | :-------- | :--- | :--- | :--------- |
| play      | `object`  | 否   |      | 玩家对象   |
| moneyname | `string`  | 否   |      | 货币名称   |
| result    | `integer` | 否   |      | 对应货币值 |

```
表：cfg_item.xls表，设置方法：Reserved字段 
货币组分类(数字)#优先扣除顺序，如：22#1 22#2 22#3
这3个货币是一个类别的，后面的1 2 3 代表扣除的顺序，数字越小越优先扣除。
```

