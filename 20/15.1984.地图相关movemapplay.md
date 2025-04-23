### 把某个地图中的玩家全部移动到另外一个地图
`movemapplay`

| 参数   | 类型      | 空   | 默认               | 注释         |
| :----- | :-------- | :--- | :----------------- | :----------- |
| play   | `object`  | 否   |                    | 玩家对象     |
| aMapId | `string`  | 否   |                    | 移动前地图Id |
| bMapId | `string`  | 否   |                    | 移动后地图Id |
| x      | `integer` | 否   |                    | x坐标        |
| y      | `integer` | 否   |                    | y坐标        |
| range  | `integer` | 否   | 引擎64_23.0830新增 | 范围         |
```lua
movemapplay(actor,0,3,333,333,5)
```

