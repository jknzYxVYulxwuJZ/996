#### 英雄角色穿戴/脱下装备前触发

`herotakeonbeforeex`~`herotakeoffbeforeex`

| 参数      | 类型      | 空   | 默认                | 注释                                |
| :-------- | :-------- | :--- | :------------------ | :---------------------------------- |
| self      | `object`  | 否   |                     | 玩家对象                            |
| item      | `object`  | 否   |                     | 物品对象                            |
| where     | `integer` | 否   | 引擎64_24.08.07新增 | 装备位置                            |
| makeIndex | `integer` | 否   | 引擎64_24.08.07新增 | 装备唯一ID                          |
| makeIndex | `integer` | 否   | 引擎64_24.08.07新增 | 英雄对象                            |
| result    | `bool`    | 否   |                     | true = 允许操作<br />false = 阻止操作 |

