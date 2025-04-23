### 命令移动怪物

`movemontopos`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.10.24新增接口&lt;/font&gt;**

| 参数    | 类型      | 空   | 默认 | 注释     |
| :------ | :-------- | :--- | :--- | :------- |
| monName | `string`  | 否   |      | 怪物名字 |
| mapID   | `string`  | 否   |      | 地图ID   |
| posX1   | `integer` | 否   |      | 老坐标X  |
| posY1   | `integer` | 否   |      | 老坐标Y  |
| posX2   | `integer` | 否   |      | 新坐标X  |
| posY2   | `integer` | 否   |      | 新坐标Y  |
```lua
    movemontopos("练功稻草人",3,300,300,333,333)
```

------------

