### 批量拿走背包物品

`takes`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.03.14新增接口&lt;/font&gt;**

| 参数    | 类型      | 空   | 默认                | 注释                                                         |
| :------ | :-------- | :--- | :------------------ | :----------------------------------------------------------- |
| play    | `object`  | 否   |                     | 玩家对象                                                     |
| itemStr | `string`  | 否   |                     | 物品#物品数量&amp;物品#物品数量 (&amp;=和的意思)                     |
| varName | `string`  | 否   |                     | 存入变量名,判断扣除道具中是否有绑定的<br />0=非绑定<br /> 1=绑定 |
| model   | `integer` | 否   |                     | 参数2中的传入的物品代表名称还是ID<br />0=道具名称<br />1=道具ID  |
| order   | `integer` | 否   |                     | 0=按照默认顺序<br />1=优先扣除绑定道具                         |
| desc    | `string`  | 是   | 引擎64_24.05.23新增 | 描述                                                         |
| result  | `bool`    | 否   |                     | 是否扣除成功                                                 |

```lua
    local varName = "N0"
    local bool = takes(actor,item_str,varName,0,0,"GM删物品")
    release_print("takes是否扣除成功:",bool)
    release_print("判断扣除道具中是否有绑定",getplaydef(actor, varName))
```

