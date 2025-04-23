#### 人物死亡装备掉落前触发

`checkdropuseitems`

| 参数    | 类型      | 空   | 默认 | 注释                                |
| :------ | :-------- | :--- | :--- | :---------------------------------- |
| actor   | `object`  | 否   |      | 玩家对象                            |
| where   | `integer` | 否   |      | 装备位                              |
| itemIdx | `integer` | 否   |      | 装备idx                             |
| result  | `bool`    | 否   |      | true = 允许掉落<br />false = 阻止掉落 |

