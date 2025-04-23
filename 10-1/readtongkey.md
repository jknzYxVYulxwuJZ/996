### 读取指定 区服 配置

&gt; 读取后由触发QF的`readtongok`函数

`readtongkey`

| 参数     | 类型     | 空   | 默认 | 注释                                         |
| :------- | :------- | :--- | :--- | :------------------------------------------- |
| serverID | `string` | 否   |      | 传入主区ID,在主区执行该命令无效              |
| path     | `string` | 否   |      | 文件路径<br />例 `'..\\QuestDiary\\996m2.txt'` |
| key      | `string` | 否   |      | 字段                                         |
| varName  | `string` | 否   |      | 变量                                         |
```lua
    local serverID = getcost("0","&lt;$MAINTONGSERVER&gt;")
    readtongkey(serverID,'..\\QuestDiary\\996m2.txt',"通区配置","A100")

    --QF触发
    function readtongok(sysobj)
        local msg = "QF触发:当前读取服务器&lt;$MAINTONGSERVER&gt;--时间戳--&lt;$UTCNOW8&gt;--读取值&lt;$str(A100)&gt;"
        release_print(parsetext(msg,sysobj))
    end
```

