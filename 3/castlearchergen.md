### 雇佣沙巴克弓箭手/卫士

`castlearchergen`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数    | 类型      | 空   | 默认 | 注释                           |
| :------ | :-------- | :--- | :--- | :----------------------------- |
| monID   | `integer` | 否   |      | 弓箭手/卫士ID                  |
| monType | `integer` | 是   | 0    | 类型<br />0/nil=弓箭手<br />1=卫士 |

&gt; 注:**雇佣弓箭手/守卫需要消耗城堡金币,可以在[M2-参数设置-城堡参数]中设置雇佣弓箭/卫士=0**
&gt; 注:**弓箭手/守卫的尸体消失后才能进行**

```lua
-- monID对应的是SabukW.txt配置中的Archer/Guard的id
-- 示例:1号弓箭手信息
-- Archer_1_X=662
-- Archer_1_Y=333
-- Archer_1_Name=弓箭手
-- Archer_1_HP=2000
-- 示例:2号护卫信息
-- Guard_2_X=649
-- Guard_2_Y=301
-- Guard_2_Name=护卫
-- Guard_2_HP=1000
function main(actor)
    for i = 1,24 do
        castlearchergen(i)
        release_print("雇佣弓箭手",i)
    end
    for i = 1,8 do
        castlearchergen(i,1)
        release_print("雇佣护卫",i)
    end
end
```
