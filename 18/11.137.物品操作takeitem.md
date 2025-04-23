### 拿物品

 `takeitem`

&gt; **&lt;font color="#FF0000" style="font-size: 13px;"&gt;注:务必判断返回值,是否扣除物品成功,引擎锁定的物品并不会被扣除!&lt;/font&gt;**

 
| 参数     | 类型      | 空   | 默认                | 注释                                       |
| :------- | :-------- | :--- | :------------------ | :----------------------------------------- |
| play     | `object`  | 否   |                     | 玩家对象                                   |
| itemName | `string`  | 否   |                     | 物品名称                                   |
| itemNum  | `integer` | 是   |                     | 数量                                       |
| IgnoreJP | `integer` | 是   |                     | 忽略极品<br />0：所有都扣除<br />1：极品不扣除 |
| desc     | `string`  | 是   | 引擎64_24.05.23新增 | 描述                                       |
| result   | `bool`    | 是   |                     | true：成功<br />false：失败                  |
```lua
if not takeitem(actor,"木剑",2) then
    return say(actor,"物品扣除失败")
end
```

