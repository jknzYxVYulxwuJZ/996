### 批量给予物品

`gives`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数    | 类型     | 空   | 默认 | 注释                                                      |
| :------ | :------- | :--- | :--- | :-------------------------------------------------------- |
| actor   | `object` | 否   |      | 玩家对象                                                  |
| itemStr | `string` | 否   |      | 物品参数<br />物品名称#数量#绑定状态&amp;物品名称#数量#绑定状态 |
| desc    | `string` | 否   |      | 描述                                                      |
```lua
    local itemStr = "木剑#1#128&amp;开天#1"
    gives(actor,itemStr,"[gives]刷物品测试")
```

