### 获取地图玩家对象列表

`getplaycount`

| 参数         | 类型           | 空   | 默认 | 注释                                      |
| :----------- | :------------- | :--- | :--- | :---------------------------------------- |
| MapId        | `string`       | 否   |      | 地图ID                                    |
| bIgnoreDied  | `integer`      | 否   |      | 是否忽略死亡角色<br />1:忽略<br />0:不忽略    |
| bIgnoreDummy | `integer`      | 否   |      | 是否忽略假人<br />1:忽略<br />0:不忽略        |
| result       | `table/string` | 否   |      | 存在玩家返回玩家列表<br />地图内无人返回"0" |

```lua
    local players = getplaycount("0",1,1)
    release_print("players",type(players))
    for index, player in ipairs(type(players) == "table" and players or {}) do
        release_print("player",index, getbaseinfo(player,1))
    end
```

