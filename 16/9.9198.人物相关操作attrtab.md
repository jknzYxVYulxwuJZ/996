### 获取角色所有属性

`attrtab`

| 参数   | 类型     | 空   | 默认 | 注释       |
| :----- | :------- | :--- | :--- | :--------- |
| play   | `object` | 否   |      | 玩家对象   |
| result | `table`  | 否   |      | 所有属性值 |
```lua
    local attr = attrtab(actor)
    for key, value in pairs(attr or {}) do
        release_print("attr",key,value)
    end
```

------------

## 骑马相关

