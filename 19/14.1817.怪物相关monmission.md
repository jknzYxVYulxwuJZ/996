### 怪物寻路/巡逻

`monmission`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.10.24新增接口&lt;/font&gt;**

| 参数   | 类型      | 空   | 默认 | 注释                                    |
| :----- | :-------- | :--- | :--- | :-------------------------------------- |
| player | `object`  | 否   |      | 怪物对象                                |
| posX   | `string`  | 否   |      | x坐标集<br />多坐标`;`分割<br />最多传入9个 |
| posY   | `string`  | 否   |      | y坐标集<br />多坐标`;`分割<br />最多传入9个 |
| modle  | `integer` | 否   |      | 0=寻路<br />1=巡逻                        |
```lua
    local mons = genmon(3,333,333,"练功稻草人",1,2)
    for _, mon in ipairs(mons or {}) do
        -- monmission(mon,"340;340;333;333","333;340;340;333",0)   -- 寻路[寻路结束后触发missionend]
        monmission(mon,"340;340;333;333","333;340;340;333",1)   -- 巡逻
    end

    --QFunction-0.lua
    function missionend(sysobj,monobj)
        release_print("missionend,寻路结束",getbaseinfo(monobj,ConstCfg.gbase.name))
    end
```

