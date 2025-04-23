### 执行自动回收

`autorecycling`

| 参数          | 类型      | 空   | 默认 | 注释                     |
| :------------ | :-------- | :--- | :--- | :----------------------- |
| actor         | `string`  | 否   |      | 玩家对象                 |
| interval      | `integer` | 是   |      | 检测间隔时间（单位：秒） |
| max_bag_space | `integer` | 是   |      | 执行回收的背包空格       |
```lua
--执行自动回收,2(间隔2秒检测一次) 10(背包格子 <= 10)
autorecycling(actor,2, 10)

--关闭自动回收
autorecycling(actor)
```
