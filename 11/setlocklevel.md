### 设置等级锁

`setlocklevel`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数  | 类型      | 空   | 默认 | 注释                                                                                       |
| :---- | :-------- | :--- | :--- | :----------------------------------------------------------------------------------------- |
| actor | `object`  | 否   |      | 玩家对象                                                                                   |
| itype | `integer` | 否   |      | 0:解除锁定<br />1锁定到达最大等级时并且不获取怪物经验<br />2:锁定到达最大等级时累积经验(int64) |
| level | `integer` | 否   |      | 锁住最大等级                                                                               |
```lua
[[
    特殊*：设置等级锁后 ,changeexp 仍然可以加经验, setbaseinfo 仍然可以突破等级限制
    特殊*：重进游戏需要重新设置
]]
    setlocklevel(actor,1,99)
```

------------

