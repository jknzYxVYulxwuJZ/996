### 增加气泡
`addbutshow`

| 参数 | 类型      | 空   | 默认 | 注释                     |
| :--- | :-------- | :--- | :--- | :----------------------- |
| play | `object`  | 否   |      | 玩家对象                 |
| ID   | `integer` | 否   |      | ID                       |
| name | `string`  | 否   |      | 显示名称                 |
| fun  | `fun`     | 否   |      | 函数名(多参数用逗号分割) |
```lua
addbutshow(actor,1,"测试气泡","@testjump,参数1,参数2,参数3")

function testjump(actor,...)
    release_print(...)
end

```
