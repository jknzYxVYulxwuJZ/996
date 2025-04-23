### 新手界面引导功能
`navigation`

| 参数   | 类型      | 空   | 默认 | 注释       |
| :----- | :-------- | :--- | :--- | :--------- |
| player | `object`  | 否   |      | 玩家对象   |
| NPCIdx | `integer` | 否   |      | 界面ID     |
| BtnIdx | `integer`/`string` | 否   |      | 按钮索引   |
| sMsg   | `string`  | 否   |      | 显示的内容 |
```lua
[[
参数2：界面ID(主界面ID;0=NPC面板;1=角色背包;2= 角色界面;3=英雄背包;40=英雄头像;200=PC端下方3个按钮;任务主窗口引导=任务的ID  9-12=商城面板 201=右下角切换按钮 202=玩家主面板 203=英雄主面板)
参数3：按钮ID(每个界面自己定义的ID)  例如：&lt;Text|id=221|x=25|y=20|color=255|size=18|text=NPC面板提示|link=@NPC面板提示&gt;  id=221就是NPC按钮ID
        当参数2=（9-12=商城面板）   参数3=商城序号ID
        当参数2=（202=玩家主面板）  参数3=人物1-6装备界面页签
        当参数2=（203=英雄主面板）  参数3=英雄1-6装备界面页签
参数4：文字内容
]]

例子一:
local str = "&lt;Text|id=221|x=25|y=20|color=255|size=18|text=NPC面板提示|link=@NPC面板提示&gt;"
say(actor,str)
navigation(actor,0,221,"引导文本")

例子二:
navigation(actor,202,1,"测试提示2")
```

