### 获取地图指定范围内的怪物对象列表
`getmapmon`

参数同 CheckRangeMonCount

| 参数    | 类型      | 空   | 默认 | 注释                           |
| :------ | :-------- | :--- | :--- | :----------------------------- |
| mapid   | `string`  | 否   |      | 地图Id                         |
| monName | `string`  | 否   |      | 怪物名，为空 or * 为检测所有怪 |
| nx      | `integer` | 否   |      | 坐标X                          |
| nx      | `integer` | 否   |      | 坐标Y                          |
| nRange  | `integer` | 否   |      | 范围                           |
| result  | `tab`     | 否   |      | 返回值，怪物对象               |

