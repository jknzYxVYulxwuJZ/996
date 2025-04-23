#### 获取对象int变量

`getobjintvar`

| 参数   | 类型      | 空   | 默认 | 注释          |
| :----- | :-------- | :--- | :--- | :------------ |
| obj    | `object`  | 否   |      | 怪物/NPC对象  |
| idx    | `integer` | 否   |      | 变量位置(1-5)|
| result | `integer` | 否   |      | 变量值        |

```lua
    -- 给怪物对象设置变量
    local mapID,x,y = getMapXY(actor)
    local mons = getobjectinmap(mapID,x,y,10,2)
    for i, mon in ipairs(mons or {}) do
        setobjintvar(mon,1,996 + i)
    end

    -- 给NPC对象设置变量
    local npc = getnpcbyindex(10001)
    setobjintvar(npc,1,996)
    release_print("npc变量",i,getobjintvar(npc,1))
```

