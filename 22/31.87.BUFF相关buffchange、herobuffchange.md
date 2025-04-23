### 玩家/英雄buff操作触发

`buffchange`/`herobuffchange`

| 参数  | 类型     | 空   | 默认 | 注释         |
| :---- | :------- | :--- | :--- | :----------- |
| actor | `object` | 否   |      | 玩家对象 |
| buffid | `integer` | 否   |      | buffID |
| groupid | `integer` | 否   |      | 组id |
| model | `integer` | 否   |      | 操作类型<br />1=新增;<br />2=更新;<br />4=删除; |

```lua
[[
    23.0830引擎新增登陆状态常量 &lt;$LOGINSTEP&gt;
    =1表示登陆前;=2表示登陆中;=3表示登陆完成
]]
function buffchange(actor, buffid, groupid, model)
    release_print("打印常量",getconst(actor,"&lt;$LOGINSTEP&gt;"))
end
```

