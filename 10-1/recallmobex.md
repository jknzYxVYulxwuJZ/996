### 召唤宝宝2

`recallmobex`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.03.14新增接口&lt;/font&gt;**

| 参数                 | 类型      | 空   | 默认 | 注释                         |
| :------------------- | :-------- | :--- | :--- | :--------------------------- |
| actor                | `string`  | 否   |      | 玩家对象                     |
| monster_name         | `string`  | 否   |      | 怪物名称                     |
| x                    | `integer` | 否   |      | 怪物当前地图出生点X          |
| y                    | `integer` | 否   |      | 怪物当前地图出生点Y          |
| level                | `integer` | 否   |      | 怪物等级                     |
| quantity             | `integer` | 否   |      | 数量                         |
| rebellion_time       | `integer` | 是   | 10   | 叛变时间(秒)<br />最低10秒     |
| auto_change_color    | `integer` | 否   |      | 是否自动变色                 |
| count                | `integer` | 否   |      | 检测时不计算该宝宝数量       |
| upgrade              | `integer` | 否   |      | 宝宝不升级                   |
| hide_master_name     | `integer` | 否   |      | 隐藏主人名                   |
| inherit_attr_percent | `integer` | 否   |      | 继承人物伤害百分比           |
| hp_value             | `integer` | 否   |      | 宝宝血量数值                 |
| buff_id              | `string`  | 否   |      | BUFF ID 多个BUFF ID用#号连接 |
```lua
    local mons = recallmobex(actor, "练功稻草人", x, y, 0, 5, 65535, 0, 1, 1, 1)
    for i, mon in ipairs(mons or {}) do
        release_print("宝宝系统",i,getbaseinfo(mon,ConstCfg.gbase.x),getbaseinfo(mon,ConstCfg.gbase.y))
    end
```

