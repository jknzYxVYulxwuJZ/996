### 骰子功能

`playdice`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.10.24新增接口&lt;/font&gt;**

| 参数     | 类型      | 空   | 默认 | 注释                                   |
| :------- | :-------- | :--- | :--- | :------------------------------------- |
| player   | `object`  | 否   |      | 玩家对象                               |
| num      | `integer` | 否   |      | 动画数量<br />比如3就是会出现3个骰子转动 |
| funcName | `string`  | 否   |      | 动画结束触发                           |
```lua
    [[骰子的显示顺序和点数 对应 私人变量 D0 D1 D2 D3 D4 D5]]
    setplaydef(actor, "D0",1)
    setplaydef(actor, "D1",2)
    setplaydef(actor, "D2",3)
    setplaydef(actor, "D3",4)
    setplaydef(actor, "D4",5)
    setplaydef(actor, "D5",6)
    playdice(actor,1,"@test_jump,传参")

    -- QFunction-0.lua
    function test_jump(actor,...)
        release_print("test_jump,qf",getbaseinfo(actor,1),...)
    end
```

------------

