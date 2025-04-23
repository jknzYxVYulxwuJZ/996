### 清掉地图某范围的怪物

`killmapmon`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数    | 类型      | 空   | 默认 | 注释                      |
| :------ | :-------- | :--- | :--- | :------------------------ |
| MapId   | `string`  | 否   |      | 地图ID                    |
| X       | `integer` | 否   |      | 坐标X                     |
| Y       | `integer` | 否   |      | 坐标Y                     |
| range   | `integer` | 否   |      | 范围                      |
| monName | `string`  | 否   |      | 怪物名<br />`*`表示所有怪物 |
| isDrop  | `integer` | 是   | 0    | 是否爆物品<br />0=不爆;1=爆 |
| isClear | `integer` | 是   | 0    | 是否清尸体<br />0=不清;1=清 |
```lua
    killmapmon( mapID,x,y, 10, "*", 0,1)
```

---

