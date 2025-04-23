### 获取字符串属性

`getattlist`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.12.07新增接口&lt;/font&gt;**
 

| 参数    | 类型     | 空   | 默认 | 注释             |
| :------ | :------- | :--- | :--- | :--------------- |
| play    | `object` | 否   |      | 玩家对象         |
| attridx | `string` | 否   |      | 自定义属性组名称 |
| result  | `string` | 否   |      | 属性字符串       |
```lua
    local attr_str = getattlist(actor,"自定义属性组1")
    release_print("attr_str",attr_str)
```

