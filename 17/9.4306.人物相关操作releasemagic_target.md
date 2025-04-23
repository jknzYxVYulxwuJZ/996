### 对目标释放技能

`releasemagic_target`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数    | 类型      | 空   | 默认 | 注释                                   |
| :------ | :-------- | :--- | :--- | :------------------------------------- |
| actor   | `object`  | 否   |      | 玩家对象                               |
| skillID | `integer` | 否   |      | 技能ID                                 |
| sType   | `integer` | 否   |      | 类型<br />1-普通技能<br />2-强化技能       |
| sLevel  | `integer` | 否   |      | 技能等级                               |
| target  | `object`  | 否   |      | 目标对象                               |
| data    | `integer` | 是   | 0    | 是否显示施法动作<br />0-不显示<br />1-显示 |
```lua
    releasemagic_target(actor,skill_id,1,skill_lv,mon,0)
```

