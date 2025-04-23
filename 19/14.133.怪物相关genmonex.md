### 刷怪(拓展)
`genmonex`

| 参数        | 类型             | 空   | 默认                | 注释                                               |
| :---------- | :--------------- | :--- | :------------------ | :------------------------------------------------- |
| mapid       | `string`         | 否   |                     | 地图id                                             |
| x           | `integer`        | 否   |                     | 坐标X                                              |
| y           | `integer`        | 否   |                     | 坐标Y                                              |
| monname     | `string`         | 否   |                     | 怪物名称                                           |
| range       | `integer`        | 否   |                     | 范围                                               |
| count       | `integer`        | 否   |                     | 数量                                               |
| owner       | `integer/object` | 否   |                     | 归属对象<br />填0则无指定归属                        |
| color       | `integer`        | 否   |                     | 颜色(0~255)                                        |
| showName    | `string`         | 否   |                     | 怪物自定义名称                                     |
| isFilt      | `integer`        | 否   |                     | 是否过滤数字<br />0过滤，1不过滤                     |
| countryName | `string`         | 否   | 引擎64_23.12.07新增 | 国家名称                                           |
| nAttack     | `integer`        | 否   | 引擎64_23.12.07新增 | 是否可攻击同国家的玩家<br />0=不可以<br />1=可以       |
| nNatMonPk   | `integer`        | 否   | 引擎64_23.12.07新增 | 不同国家怪物是否可PK<br />0=不可以<br />1=可以         |
| nPlayerPk   | `integer`        | 否   | 引擎64_23.12.07新增 | 人物是否可以攻击相同国家怪物<br />0=可以<br />1=不可以 |
| nNg         | `integer`        | 否   | 引擎64_23.12.07新增 | 是否是内功怪<br />0=普通怪<br />1=内功怪               |
| result      | `table`          | 否   |                     | 返回怪物列表                                       |
```lua
    genmonex(3,333,333,"神兽",1,2,0,255,"神兽\\(新)",1)

    local countryName = "华夏"
    local mons = genmonex(mapID,x,y,"练功稻草人",10,5,0,255,string.format("稻草人[%s]",countryName),1,countryName,1,1,1,1)
    for _, mon in ipairs(mons or {}) do
        release_print("========================")
        release_print("monName",getbaseinfo(mon,1,0))
        release_print("monPosM",getbaseinfo(mon,1,4),getbaseinfo(mon,1,5))
    end
```

