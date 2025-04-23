### 获取对面人物的名字
`getoppositeobj`

| 参数 | 类型     | 空   | 默认 | 注释     |
| :--- | :------- | :--- | :--- | :------- |
| play | `object` | 否   |      | 玩家对象 |
```lua
    local otherPlayer = getoppositeobj(actor)
    release_print("对面玩家",getbaseinfo(otherPlayer,1))
```

