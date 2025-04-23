### 获取IP地址下所有的在线角色名称列表

`getplaylistbyip`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.03.14新增接口&lt;/font&gt;**

| 参数          | 类型     | 空   | 默认 | 注释                                       |
| :------------ | :------- | :--- | :--- | :----------------------------------------- |
| IPAddress     | `string` | 否   |      | IP地址                                     |
| getAllPlayers | `number` | 否   | 0    | 是否获取全部玩家列表0/1(默认限制返回200个) |
```lua
    local varName = "S1"
    local ipstr = getconst(actor,"&lt;$IPADDR&gt;")
    -- callscriptex(actor,"getplaylistbyip",ipstr,varName)
    local list = getplaylistbyip(ipstr,0)
    -- local list = getplaydef(actor,varName)
    release_print("list",ipstr,tbl2json(list))
```

------------

