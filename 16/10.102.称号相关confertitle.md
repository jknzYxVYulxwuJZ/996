### 添加称号
`confertitle`

| 参数   | 类型      | 空   | 默认 | 注释            |
| :----- | :-------- | :--- | :--- | :-------------- |
| play   | `object`  | 否   |      | 玩家对象        |
| name   | `string`  | 否   |      | 称号物品名称    |
| use    | `integer` | 否   |      | 开启激活，1激活 |
| result | `bool`    | 否   |      | 是否成功        |

```lua
function main(self)
    if confertitle(self, '君临天下') then
        say(self,"添加成功")
    else
        say(self,"添加失败")
    end
end
```

