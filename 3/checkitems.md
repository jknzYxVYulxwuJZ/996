### 批量检测背包物品

`checkitems`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.03.14新增接口&lt;/font&gt;**

| 参数    | 类型      | 空   | 默认 | 注释                                                        |
| :------ | :-------- | :--- | :--- | :---------------------------------------------------------- |
| play    | `object`  | 否   |      | 玩家对象                                                    |
| itemStr | `string`  | 否   |      | 物品名称#物品数量&amp;物品名称#物品数量 (&amp;=和的意思)            |
| isBind  | `integer` | 否   |      | 0=不检测;<br /> 1.非绑定<br />2.绑定                            |
| model   | `integer` | 否   |      | 参数2中的物品名称是ID还是道具名称<br />0=道具名称<br />1=道具ID |
| result  | `bool`    | 否   |      | 是否满足条件                                                |
```lua
    local item_str = "屠龙#3&amp;木剑#4"
    if checkitems(actor,item_str ,0 ,0) then
        local bool = takes(actor,item_str,0,0)
        LOGPrint("是否扣除成功,takes",bool)
    end
```

