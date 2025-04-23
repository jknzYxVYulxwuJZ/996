### 获取阵营ID

`getcamp`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.08.07新增接口&lt;/font&gt;**

| 参数   | 类型      | 空   | 默认 | 注释     |
| :----- | :-------- | :--- | :--- | :------- |
| actor  | `object`  | 否   |      | 玩家/怪物对象 |
| result | `integer` | 否   |      | 阵营id   |
```lua
    local camp_id = getcamp(actor)
```
