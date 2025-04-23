### 改变行会名称

`changeguildname`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.03.14新增接口&lt;/font&gt;**

| 参数         | 类型     | 空   | 默认 | 注释             |
| :----------- | :------- | :--- | :--- | :--------------- |
| actor        | `string` | 否   |      | 玩家对象         |
| guildName    | `string` | 否   |      | 需要改名的行会名 |
| newGuildName | `string` | 否   |      | 新的行会名字     |

```lua
--行会改名成功
function changeguildnameok(...)
    LOGPrint("changeguildnameok,成功",...)
end
--行会改名失败,model:0=参数错误;1=原行会找不到;2=名字不合法;3=新名字重复
function changeguildnamefail(guild,model,...)
    LOGPrint("changeguildnamefail,失败",getbaseinfo(guild,1),"model:"..model,...)
end

changeguildname(actor,guildName,newName)
```

