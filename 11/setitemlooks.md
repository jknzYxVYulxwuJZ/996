### 修改装备内观Looks值

`setitemlooks`

| 参数    | 类型      | 空   | 默认                | 注释                     |
| :------ | :-------- | :--- | :------------------ | :----------------------- |
| play    | `object`  | 否   |                     | 玩家对象                 |
| itemPos | `integer` | 否   |                     | 装备位置(-2操作物品对象) |
| char    | `string`  | 否   |                     | 操作符(+ - =)            |
| pictrue | `integer` | 否   |                     | 内观图片                 |
| item    | `object`  | 否   | 引擎64_23.08.30新增 | 物品对象                 |
```lua
--根据装备位设置内观Looks值
setitemlooks(actor,1,"=",85)

--根据装备对象设置内观Looks值
setitemlooks(actor,-2,"=",85,itemobj)
```

