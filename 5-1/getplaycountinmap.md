### 获取指定地图玩家数量
`getplaycountinmap`

| 参数      | 类型      | 空   | 默认 | 注释                                         |
| :-------- | :-------- | :--- | :--- | :------------------------------------------- |
| play      | `object`  | 否   |      | 玩家对象<br />可传入系统对象`"0"`              |
| MapId     | `string`  | 否   |      | 地图ID                                       |
| isAllgain | `integer` | 否   |      | 是否全部获取<br />0=全部获取<br />1=排除已死亡的 |
| result    | `integer` | 否   |      | 返回值，玩家数量                             |
```lua
    local playerNum = getplaycountinmap("0","3",0)
    release_print("playerNum",playerNum)
```

