### 删除系统延时回调

`grobalcleardelaygoto`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数     | 类型     | 空   | 默认 | 注释                                                                       |
| :------- | :------- | :--- | :--- | :------------------------------------------------------------------------- |
| funcName | `string` | 是   |      | 需要删除的延时函数<br />不填为清除全部                                       |
| value    | `string` | 是   | 0    | 是否忽视标签参数<br />0=不忽视,要完整填写添加时的参数<br />1=忽视,只判断函数名 |
```lua
    grobaldelaygoto(1000,"grobal_jump,a,b,c")

    grobalcleardelaygoto("grobal_jump,a,b,c",0)
    grobalcleardelaygoto("grobal_jump",1)
```

