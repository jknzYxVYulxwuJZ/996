### 导航玩家到指定位置

&gt; 自动寻路到指定坐标

`gotonow`

| 参数 | 类型      | 空   | 默认 | 注释     |
| :--- | :-------- | :--- | :--- | :------- |
| play | `object`  | 否   |      | 玩家对象 |
| X    | `integer` | 否   |      | X坐标    |
| Y    | `integer` | 否   |      | Y坐标    |

```lua
gotonow(actor,330, 330) 

--QFunction-0.lua

--寻路开启
function findpathbegin(actor)
     release_print("findpathstop",getbaseinfo(actor,1),getconst(actor, "&lt;$ToPointX&gt;"),getconst(actor, "&lt;$ToPointY&gt;"))
end
--寻路中断
function findpathstop(actor)
    release_print("findpathstop",getbaseinfo(actor,1))
end
--寻路结束
function findpathend(actor)
    release_print("findpathend",getbaseinfo(actor,1))
end
```

## 镜像地图

