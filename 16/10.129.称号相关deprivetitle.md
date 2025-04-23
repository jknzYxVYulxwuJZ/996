### 删除称号

`deprivetitle`

| 参数   | 类型     | 空   | 默认 | 注释         |
| :----- | :------- | :--- | :--- | :----------- |
| play   | `object` | 否   |      | 玩家对象     |
| name   | `string` | 否   |      | 称号物品名称 |
| result | `bool`   | 否   |      | 是否成功     |
```lua
function main(play)
    if deprivetitle(play, '君临天下') then
        say(play,"删除成功")
    else
        say(play,"删除失败")
    end
end
```

