### 获取人物伤害吸收
`getsuckdamage`

| 参数   | 类型      | 空   | 默认 | 注释       |
| :----- | :-------- | :--- | :--- | :--------- |
| play   | `object`  | 否   |      | 玩家对象   |
| result | `integer` | 否   |      | 伤害吸收值 |
```lua
    setsuckdamage(actor,"=",1000,200,95)
    local damage = getsuckdamage(actor)
    release_print("伤害吸收值",damage)
```

------------

