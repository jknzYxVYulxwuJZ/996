### 接口发起行会战

`setguildwar`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.08.07新增接口&lt;/font&gt;**

| 参数       | 类型      | 空   | 默认 | 注释         |
| :--------- | :-------- | :--- | :--- | :----------- |
| guildName1 | `string`  | 否   |      | 宣战行会名字 |
| guildName2 | `string`  | 否   |      | 敌对行会名字 |
| time       | `integer` | 否   |      | 时间(分)     |
| result     | `bool`    | 否   |      | 是否发起成功 |
```lua
    local bool = setguildwar(guildName_1,guildName_2,30)
```

