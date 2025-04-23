#### 获取对象str变量

`getobjstrvar`

| 参数   | 类型      | 空   | 默认 | 注释          |
| :----- | :-------- | :--- | :--- | :------------ |
| obj    | `object`  | 否   |      | 怪物/NPC对象  |
| idx    | `integer` | 否   |      | 变量位置(1-5)|
| result | `string`  | 否   |      | 变量值        |

```lua
    -- 给怪物对象设置变量
    local mapID,x,y = getMapXY(actor)
    local mons = getobjectinmap(mapID,x,y,10,2)
    for i, mon in ipairs(mons or {}) do
        setobjstrvar(mon,1,"996monValue_" .. i)
        release_print("怪物变量",i,getobjstrvar(mon,1))
    end

    -- 给NPC对象设置变量
    local npc = getnpcbyindex(10001)
    setobjstrvar(npc,1,"996npcValue")
    release_print("npc变量",i,getobjstrvar(npc,1))
```

------------
## 地图变量

&gt; **临时变量,不会存储数据库**

