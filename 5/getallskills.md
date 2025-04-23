### 接口获取角色所有技能

`getallskills`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.08.07新增接口&lt;/font&gt;**

| 参数   | 类型     | 空   | 默认 | 注释     |
| :----- | :------- | :--- | :--- | :------- |
| actor  | `object` | 否   |      | 玩家对象 |
| result | `table`  | 否   |      | 技能列表 |
```lua
    local skill_list = getallskills(actor)
    for _, skillID in ipairs(skill_list or {}) do
        release_print("技能", skillID )
    end
```

------------

