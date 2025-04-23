### 绑定背包满触发

`bindevent`

| 参数         | 类型      | 空   | 默认 | 注释                       |
| :----------- | :-------- | :--- | :--- | :------------------------- |
| play         | `object`  | 否   |      | 玩家对象                   |
| bindingType  | `object`  | 否   |      | 绑定类型(1：背包满通知)    |
| isOpen       | `integer` | 否   |      | 是否开启(0：关闭，1：开启) |
| callbackFunc | `string`  | 否   |      | 回调函数(QF)               |

```lua
bindevent(actor,1,1,"@on_bag_full_lua")

--QFunction-0.lua
function on_bag_full_lua(actor,...)
end
```

------------

