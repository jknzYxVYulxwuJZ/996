### 设置buff堆叠层数

`buffstack`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数   | 类型      | 空   | 默认 | 注释                          |
| :----- | :-------- | :--- | :--- | :---------------------------- |
| actor  | `object`  | 否   |      | 对象                          |
| buffid | `integer` | 否   |      | buffid                        |
| opt    | `string`  | 否   |      | 操作符 "+" "-" "="            |
| stack  | `integer` | 否   |      | buff层数 不可超出表中最大层数 |
| itimer | `boolean` | 否   |      | 是否重置buff 时间             |
```lua
  buffstack(actor,10000,"+",1,true)
```
