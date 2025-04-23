### 获取指定地图怪物数量
`getmoncount`

| 参数     | 类型      | 空   | 默认 | 注释                                        |
| :------- | :-------- | :--- | :--- | :------------------------------------------ |
| MapId    | `string`  | 否   |      | 地图ID                                      |
| MonId    | `integer` | 否   |      | 怪物id<br />传入-1获取所有怪物                |
| isAllMon | `boolean` | 否   |      | 是否忽略宝宝<br /> true:忽略<br /> false:不忽略 |
| result   | `integer` | 否   |      | 返回值，怪物数量                            |

