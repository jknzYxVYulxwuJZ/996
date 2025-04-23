### 指定怪物的爆出

`monitemsex`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数      | 类型      | 空   | 默认 | 注释                       |
| :-------- | :-------- | :--- | :--- | :------------------------- |
| actor     | `object`  | 否   |      | 玩家对象                   |
| monItem   | `string`  | 否   |      | 怪物名称                   |
| value     | `integer` | 否   |      | 可爆出次数<br />最大多爆20次 |
| delayTime | `integer` | 是   | 0    | 延迟毫秒数                 |
```lua
--接口需要杀怪触发[killmon]中使用
function killmon(actor, monobj)
    if getbaseinfo(monobj,1) == "食人花" then
        monitemsex(actor,"练功稻草人",2,5000)
    end
end
```

---

