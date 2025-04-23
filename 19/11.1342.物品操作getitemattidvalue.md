### 获取人物身上装备属性值命令

`getitemattidvalue`

| 参数   | 类型      | 空   | 默认 | 注释                                  |
| :----- | :-------- | :--- | :--- | :------------------------------------ |
| play   | `object`  | 否   |      | 玩家对象                              |
| model  | `integer` | 否   |      | 类型(1，装备表里基础数据 2，附加属性) |
| attrID | `integer` | 否   |      | 属性ID                                |
| where  | `integer` | 否   |      | 装备位置(-2操作物品对象)              |
| item   | `object`  | 否   |      | 物品对象                              |
```lua
--根据装备位获取属性
local attr_str = getitemattidvalue(actor,2,4,1)

--根据物品对象获取属性
local attr_str = getitemattidvalue(actor,2,4,-2,itemobj)
```

------------

## 宝石相关
