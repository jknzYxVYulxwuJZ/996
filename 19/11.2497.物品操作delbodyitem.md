### 从装备位扣除物品

`delbodyitem`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.10.24新增接口&lt;/font&gt;**

| 参数   | 类型      | 空   | 默认                | 注释                            |
| :----- | :-------- | :--- | :------------------ | :------------------------------ |
| player | `object`  | 否   |                     | 玩家对象                        |
| where  | `integer` | 否   |                     | 装备位                          |
| desc   | `string`  | 是   | 引擎64_24.05.23新增 | 描述                            |
| result | `bool`    | 是   |                     | true=扣除成功<br />false=扣除失败 |

