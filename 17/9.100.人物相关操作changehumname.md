### 修改人物名称

`changehumname`

| 参数   | 类型      | 空   | 默认 | 注释                                                                                               |
| :----- | :-------- | :--- | :--- | :------------------------------------------------------------------------------------------------- |
| play   | `object`  | 否   |      | 玩家对象                                                                                           |
| name   | `string`  | 否   |      | 要查询的名字                                                                                       |
| result | `integer` |      |      | 执行结果：<br />0-改名成功<br />1、2、6-名称被过滤<br />3-名字已经存在<br />5-长度不符合要求<br />7-改名失败 |
```lua
1. 会先执行查询人物名称操作，并触发：queryinghumname;
2. 会根据查询结果情况触发：humnamefilter（名称被过滤）、namelengthfail（长度不符合要求）、humnameexists（名称已经存在）;
3. 执行改名操作前触发：changeinghumname，根据改名结果触发：changehumnameok(改名成功)、changehumnamefail(改名失败)。
	
--正在查询玩家名称
function queryinghumname(actor)
    sendmsg(actor, 1, '{"Msg":"&lt;font color=\'#ff0000\'&gt;正在查询请稍后。。。&lt;/font&gt;","Type":9}')
end

--名称被过滤
function humnamefilter(actor)
    sendmsg(actor, 1, '{"Msg":"&lt;font color=\'#ff0000\'&gt;名称被过滤。。。&lt;/font&gt;","Type":9}')
end

--长度不符合要求
function namelengthfail(actor)
    sendmsg(actor, 1, '{"Msg":"&lt;font color=\'#ff0000\'&gt;长度不符合要求&lt;/font&gt;","Type":9}')
end

--名称已经存在
function humnameexists(actor)
    sendmsg(actor, 1, '{"Msg":"&lt;font color=\'#ff0000\'&gt;名称已经存在&lt;/font&gt;","Type":9}')
end

--正在执行改名操作
function changeinghumname(actor)
    sendmsg(actor, 1, '{"Msg":"&lt;font color=\'#ff0000\'&gt;正在修改请稍后。。。&lt;/font&gt;","Type":9}')
end

--改名成功
function changehumnameok(actor)
    sendmsg(actor, 1, '{"Msg":"&lt;font color=\'#ff0000\'&gt;'..parsetext("你的名字修改成功，旧名称：&lt;$USERNAME&gt; 新名称：&lt;$USERNEWNAME&gt;！",actor)..'&lt;/font&gt;","Type":9}')
end

--改名失败
function changehumnamefail(actor)
    sendmsg(actor, 1, '{"Msg":"&lt;font color=\'#ff0000\'&gt;修改名称失败&lt;/font&gt;","Type":9}')
end
```

