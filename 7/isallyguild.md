### 判断行会之间是否结盟

`isallyguild`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.08.07新增接口&lt;/font&gt;**

| 参数       | 类型     | 空   | 默认 | 注释              |
| :--------- | :------- | :--- | :--- | :---------------- |
| guildName1 | `string` | 否   |      | 行会名字/行会对象 |
| guildName2 | `string` | 否   |      | 行会名字/行会对象 |
| result     | `bool`   | 否   |      | 是否宣战          |
```lua
    local bool_1 = isallyguild(guild_1,guild_2)
    local bool_2 = isallyguild(guildName_1,guildName_2)
    LOGPrint("是否是结盟关系",bool_1,bool_2)
```
