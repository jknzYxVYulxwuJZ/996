### 移动到指定NPC附近
`opennpcshowex`

| 参数     | 类型     | 空   | 默认 | 注释                                    |
| :------- | :------- | :--- | ---- | --------------------------------------- |
| play     | `object` | 否   |      | 玩家对象                                |
| NPCIndex | `int`    | 否   |      | NPC索引（NPC配置表中的ID）              |
| nRange   | `int`    | 否   |      | 范围值，<br>不在此范围内则移动到NPC附近 |
| nRange2  | `int`    | 否   |      | 范围值2，移动到NPC附近的范围内          |
```
1. NPC不在当前地图时: nRange>0: 瞬移传送到NPC附近; nRange=0: 不传送;
2. NPC在当前地图时: nRange>0: 瞬移传送到NPC附近; nRange=0: 导航到NPC附近;
```

