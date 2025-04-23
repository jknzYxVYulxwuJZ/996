### 获取角色所有分身
`clonelist`

| 参数   | 类型     | 空   | 默认 | 注释         |
| :----- | :------- | :--- | :--- | :----------- |
| play   | `object` | 否   |      | 玩家对象     |
| result | `table`  |      |      | 玩家分身列表 |
```lua
        local selflist = clonelist(actor)
        for i, _self in ipairs(selflist or {}) do
            release_print("分身列表",i,getbaseinfo(_self,1))
        end
```

