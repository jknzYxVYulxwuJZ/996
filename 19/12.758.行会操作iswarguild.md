### 判断行会之间是否宣战

`iswarguild`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.08.07新增接口&lt;/font&gt;**

| 参数       | 类型     | 空   | 默认 | 注释              |
| :--------- | :------- | :--- | :--- | :---------------- |
| guildName1 | `string` | 否   |      | 行会名字/行会对象 |
| guildName2 | `string` | 否   |      | 行会名字/行会对象 |
| result     | `bool`   | 否   |      | 是否宣战          |
```lua
    --传入行会对象
    local bool_1 = iswarguild(guild_1,guild_2)
    --传入行会名称
    local bool_2 = iswarguild(guildName_1,guildName_2)
    LOGPrint("是否是宣战关系",bool_1,bool_2)
```

