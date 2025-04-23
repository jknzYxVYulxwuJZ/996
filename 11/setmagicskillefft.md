### 改变技能特效

`setmagicskillefft`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.12.07新增接口&lt;/font&gt;**

| 参数      | 类型      | 空   | 默认 | 注释                                                    |
| :-------- | :-------- | :--- | :--- | :------------------------------------------------------ |
| play      | `object`  | 否   |      | 玩家对象                                                |
| skillName | `string`  | 否   |      | 技能名称                                                |
| effectID  | `integer` | 否   |      | 特效id,=0为关闭<br />(cfg_skill_present.xls表id)          |
| effectID2 | `integer` | 否   |      | 持续性ID(魔法盾BUFF表id/火墙/群体雷电术/其他的技能无效) |
```lua
    setmagicskillefft(actor,"雷电术", 33)
```

------------

## 获取玩家对象

