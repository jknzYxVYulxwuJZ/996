### 让怪物释放自定义技能

`mon_docustommagic`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**
&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;注：只支持自定义怪物（race=156，RaceImg=19）&lt;/font&gt;**

| 参数    | 类型      | 空   | 默认 | 注释         |
| :------ | :-------- | :--- | :--- | :----------- |
| actor   | `object`  | 否   |      | 怪物对象     |
| skillID | `integer` | 否   |      | 自定义技能id |
| X       | `integer` | 否   |      | 目标点X坐标  |
| Y       | `integer` | 否   |      | 目标点Y坐标  |
| target  | `object`  | 否   |      | 目标对象     |

```lua
    mon_docustommagic(mon,skill_id,pos_X,pos_Y,actor)
```

