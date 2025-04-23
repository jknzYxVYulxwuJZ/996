### 创建临时NPC
`createnpc`

| 参数 | 类型      | 空   | 默认 | 注释                  |
| :--- | :-------- | :--- | ---- | --------------------- |
| map  | `string`  | 否   |      | 地图编号              |
| X    | `integer` | 否   |      | X坐标                 |
| Y    | `integer` | 否   |      | Y坐标                 |
| NPC  | `string`  | 否   |      | NPC信息<br>json字符串 |

```lua
[[
    注意：自定义NPC的Idx不允许与配置表中的NPCID重复。
    Idx重复的NPC不会被创建出来。
]]
local npcInfo = {
    ["Idx"] =  npcidx,  -- 自定义NPC的Idx，NPC点击触发时，触发参数会传回Idx值
    ["npcname"] =  "测试", -- NPC名称
    ["appr"] =   7,  -- NPC外形效果
    ["script"] =   'NewNPC'  -- NPC相关脚本名称，表示Envir\Market_def\NewNPC.txt
    ["limit"] = 5, -- 生命周期 (秒) 引擎64_24.05.23新增
}
createnpc(mapID,x,y,tbl2json(npcInfo))

```

