### 调整人物的当前内力值

`addinternalforce`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.12.07新增接口&lt;/font&gt;**

| 参数  | 类型      | 空   | 默认 | 注释                           |
| :---- | :-------- | :--- | :--- | :----------------------------- |
| play  | `object`  | 否   |      | 玩家对象                       |
| sFlag | `string`  | 否   |      | 操作符(=,+,-)                  |
| value | `integer` | 否   |      | 内力值                         |
| model | `integer` | 否   |      | 计算方式<br />0=点数<br />1=万分比 |
```lua
    addinternalforce(actor,"+",1,0)
```
