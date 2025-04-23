### 添加组队成员触发

`groupaddmember`

| 参数   | 类型     | 空   | 默认 | 注释     |
| :----- | :------- | :--- | :--- | :------- |
| actor1 | `object` | 否   |      | 玩家对象 |
```lua
--允许主动申请加入队伍成员入队
function groupaddmember(actor)
    say(actor,"被允许进组的玩家"..getplaydef(actor,"S0"))
end
```

