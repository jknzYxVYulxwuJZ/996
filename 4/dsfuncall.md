##### 增加系统任务计时

`dsfuncall`

> **<font color="#808080" style="font-size: 13px;">引擎64_23.10.24新增接口</font>**

| 参数     | 类型      | 空   | 默认 | 注释                                       |
| :------- | :-------- | :--- | :--- | :----------------------------------------- |
| player   | `object`  | 否   |      | 玩家对象                                   |
| funcName | `string`  | 否   |      | 回调函数名<br>需以`dingshicf_`开头         |
| time     | `integer` | 否   |      | 倒计时时间(毫秒)                           |
| model    | `integer` | 否   |      | 0=上线需重新开启否则消失<br>1=上线直接执行 |
| isClear  | `integer` | 否   |      | 0=开启新的<br>1=上线刷新当前时间           |
```lua
 --QFunction-0.lua
function dingshicf_1(actor)
end

dsfuncall(actor,"dingshicf_1",10 * 1000 ,1 ,1)
```

