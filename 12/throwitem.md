### 在地图上放置物品

`throwitem`

| 参数      | 类型      | 空   | 默认               | 注释                                                           |
| :-------- | :-------- | :--- | :----------------- | :------------------------------------------------------------- |
| play      | `object`  | 否   |                    | 玩家对象                                                       |
| MapId     | `string`  | 否   |                    | 地图ID                                                         |
| X         | `integer` | 否   |                    | 坐标X                                                          |
| Y         | `integer` | 否   |                    | 坐标Y                                                          |
| range     | `integer` | 否   |                    | 范围                                                           |
| itemName  | `string`  | 否   |                    | 物品名                                                         |
| count     | `integer` | 否   |                    | 数量                                                           |
| time      | `integer` | 否   |                    | 时间（秒）                                                     |
| hint      | `bool`    | 否   |                    | 是否掉落提示                                                   |
| take      | `bool`    | 否   |                    | 是否立即拾取                                                   |
| onlyself  | `bool`    | 否   |                    | 仅自己拾取                                                     |
| xyinorder | `bool`    | 否   |                    | 是-按位置顺序，<br />否-随机位置                                 |
| overlap   | `integer` | 否   | 引擎64_23.0830新增 | 单个物品叠加数量，装备无效                                     |
| isAuto    | `bool`    | 否   | 引擎64_23.0830新增 | true=可自动拾取<br />false=不可自动拾取<br />(onlyself=true时生效) |

