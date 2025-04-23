### 删除组队成员触发

`groupdelmember`

| 参数  | 类型     | 空   | 默认 | 注释     |
| :---- | :------- | :--- | :--- | :------- |
| actor | `object` | 否   |      | 队长对象 |
```lua
--队长删除小组成员
--actor     队长人物对象
function groupdelmember(actor)
    say(actor,"被踢玩家名"..getplaydef(actor,"S0"))
end
```

