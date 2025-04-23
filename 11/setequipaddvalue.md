### 设置装备部位属性加成(万分比)

 `setequipaddvalue`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.12.07新增接口&lt;/font&gt;**
 
| 参数  | 类型      | 空   | 默认 | 注释          |
| :---- | :-------- | :--- | :--- | :------------ |
| play  | `object`  | 否   |      | 玩家对象      |
| where | `integer` | 否   |      | 装备部位      |
| sFlag | `string`  | 否   |      | 操作符(=,+,-) |
| pro   | `integer` | 是   |      | 倍数(万分比)  |
```lua
setequipaddvalue(actor,1 ,"+", 15000)
say(actor,"武器部位的属性加成".. getequipaddvalue(actor,1))
```

