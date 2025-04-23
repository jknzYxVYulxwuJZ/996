### 拿物品(拓展)

 `takeitemex`

&gt; **&lt;font color="#FF0000" style="font-size: 13px;"&gt;注:务必判断返回值,是否扣除物品成功,引擎锁定的物品并不会被扣除!&lt;/font&gt;**

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.12.07新增接口&lt;/font&gt;**
 
| 参数     | 类型      | 空   | 默认 | 注释                                         |
| :------- | :-------- | :--- | :--- | :------------------------------------------- |
| play     | `object`  | 否   |      | 玩家对象                                     |
| itemName | `string`  | 否   |      | 物品名称                                     |
| itemNum  | `integer` | 是   |      | 数量                                         |
| bind     | `integer` | 是   |      | 0=忽略<br />1=扣除非绑定物品<br />2=扣除绑定物品 |
| desc     | `string`  | 是   |      | 描述                                         |
| result   | `bool`    | 是   |      | true：成功<br />false：失败                    |
```lua
if not takeitemex(actor, "木剑", 3,1,"奖励") then
    return say(actor,"物品扣除失败")
end
```

