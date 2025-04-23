#### 角色穿戴/脱下装备前触发

`takeonbeforeex`~`takeoffbeforeex`

| 参数      | 类型      | 空   | 默认                | 注释                                |
| :-------- | :-------- | :--- | :------------------ | :---------------------------------- |
| self      | `object`  | 否   |                     | 玩家对象                            |
| item      | `object`  | 否   |                     | 物品对象                            |
| where     | `integer` | 否   | 引擎64_23.10.24新增 | 装备位置                            |
| makeIndex | `integer` | 否   | 引擎64_23.10.24新增 | 装备唯一ID                          |
| result    | `bool`    | 否   |                     | true = 允许操作<br />false = 阻止操作 |

`takeonbefore(X)`~`takeoffbefore(X)`

&gt; X=装备位置

| 参数   | 类型     | 空   | 默认 | 注释                                |
| :----- | :------- | :--- | :--- | :---------------------------------- |
| self   | `object` | 否   |      | 玩家对象                            |
| item   | `object` | 否   |      | 物品对象                            |
| result | `bool`   | 否   |      | true = 允许操作<br />false = 阻止操作 |

