### 邀请组队前触发

`invitegroup`

| 参数   | 类型      | 空   | 默认 | 注释         |
| :----- | :-------- | :--- | :--- | :----------- |
| actor1 | `object`  | 否   |      | 发起邀请对象 |
| actor2 | `object`  | 否   |      | 被邀请对象   |
| result | `integer` | 否   |      | 是否允许邀请 |
```lua
function invitegroup(actor,role)
    if getbaseinfo(role,6) &lt; 50 then
        say(actor,"被邀请玩家等级不到50级")
        return false
    end
    return true
end
```

