### buff触发血量改变时

`bufftriggerhpchange`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增触发&lt;/font&gt;**

&lt;font color="#ff00ff" style="font-family: Fixedsys;font-size: 15px;"&gt;特殊：该触发中不允许直接删除buff，包括buff组关系等影响的删除(会内存泄漏)&lt;/font&gt;
&lt;font color="#ff00ff" style="font-family: Fixedsys;font-size: 15px;"&gt;特殊：如果一定要删除请使用延时回调&lt;/font&gt;

| 参数      | 类型      | 空   | 默认 | 注释                                     |
| :-------- | :-------- | :--- | :--- | :--------------------------------------- |
| actor     | `object`  | 否   |      | 玩家对象<br />buff触发者为怪物时,该参数无效 |
| buffID    | `integer` | 否   |      | buffid                                   |
| buffGroup | `integer` | 否   |      | buff组                                   |
| HP        | `integer` | 否   |      | hp                                       |
| buffHost  | `object`  | 否   |      | 释放者对象                               |
| mon       | `object`  | 是   |      | 怪物对象<br />buff触发者为玩家时,该参数无效 |
| result    | `integer` | 否   |      | 本次扣血                                 |

```lua
    function bufftriggerhpchange(actor,buffID,buffGroup,hp,buffHost,mon)
        return hp
    end
```

------

## 接口

