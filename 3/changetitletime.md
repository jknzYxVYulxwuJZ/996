### 改变称号时间

`changetitletime`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.03.14新增接口&lt;/font&gt;**

| 参数      | 类型      | 空   | 默认 | 注释                                   |
| :-------- | :-------- | :--- | :--- | :------------------------------------- |
| actor     | `string`  | 否   |      | 玩家对象                               |
| titleName | `string`  | 否   |      | 称号名称                               |
| operation | `string`  | 否   |      | 操作符（+,-,=）                        |
| cour      | `integer` | 否   |      | 时间(+,-传入操作时间(秒), =传入时间戳) |

```lua
    changetitletime(actor,titleName,"+",cour)
```

------------

