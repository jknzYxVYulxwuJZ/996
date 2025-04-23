### 获取当前地图行会成员数量

`maphanghcyguild`

| 参数      | 类型     | 空   | 默认 | 注释                              |
| :-------- | :------- | :--- | :--- | :-------------------------------- |
| mapID     | `string` | 否   |      | 地图编号                          |
| guildName | `string` | 否   |      | 行会名字或 * (等于未加入行会角色) |

```lua
local num = maphanghcyguild(3,"*")
```

