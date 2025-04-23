### 获取所有玩家对象列表(遍历玩家列表)

`getplayerlst`

| 参数    | 类型      | 空   | 默认                | 注释                                           |
| :------ | :-------- | :--- | :------------------ | :--------------------------------------------- |
| offline | `integer` | 是   | 引擎64_24.05.23新增 | 是否剔除离线挂机玩家<br />0/nil=不剔除<br />1=剔除 |

```lua
    local player_list = getplayerlst(0)
    for i, player  in ipairs(player_list or {}) do
        release_print("在线玩家",i,getbaseinfo(player,1),"角色是否离线挂机:",getbaseinfo(player,61))
    end
```

------------

