### 获取怪物原始各项数据库字段值参数

`getdbmonfieldvalue`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.10.24新增接口&lt;/font&gt;**

| 参数           | 类型               | 空   | 默认 | 注释               |
| :------------- | :----------------- | :--- | :--- | :----------------- |
| monIdx/monName | `integer`/`string` | 否   |      | 怪物ID/怪物名称    |
| fieldName      | `string`           | 否   |      | 字段名(看下方示例) |
| result         | `string`           | 否   |      | 表格数据           |
```lua
    local config = {
        {"idx","0列"},
        {"name","1列"},
        {"race","2列"},
        {"raceimg","3列"},
        {"appr","4列"},
        {"level","5列"},
        {"lifeattrib","6列"},
        {"cooleye","7列"},
        {"exp","8列"},
        {"hp","9列","生命值"},
        {"mp","9列","魔法值"},
        {"dc","9列","攻击下限"},
        {"maxdc","9列","攻击上限"},
        {"mc","9列","魔法"},
        {"sc","9列","道术"},
        {"ac","9列","物防下限"},
        {"ac1","9列","物防上限"},
        {"mac","9列","魔防下限"},
        {"mac1","9列","魔防上限"},
        {"speed","10列"},
        {"hitpoint","11列"},
        {"walkspeed","12列"},
        {"walkstep","13列"},
        {"walkwait","14列"},
        {"attackspeed","15列"},
        {"attribute","16列"},
        {"color","17列"},
        {"rehealthcd","18列"},
        {"type","19列"},
        {"viewrange","20列"},
        {"droptype","21列"},
        {"through","22列"},
        {"isboss","23列"},
        {"homerate","24列"},
        {"monparam1","25列"},
        {"attacklist","26列"},
        {"bigtipid","27列"},
        {"noshow","28列"},
        {"isngmon","29列"},
        {"bodyleathery","30列"},
        {"butchrate","30列"},
    }
    for _, v in ipairs(config) do
        release_print("对应monster表",v[2],v[1]..(v[3] or ""),getdbmonfieldvalue("[BOSS]沃玛教主3",v[1]))
    end
```

------------

