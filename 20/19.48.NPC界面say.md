### NPC界面文本发送
`say`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|actor     |`object`      |否   |    |   玩家对象 |
|msg     |`string`      |否   |    |  界面文本内容  |

```lua
function main(actor)
    local msg = [[
        <Button|a=0|x=180.0|y=2.0|tips={点击查看【金钻服务】/FCOLOR=250}|tipsx=10|tipsy=110|nimg=public/00000361.png|color=255|size=18|pimg=public/00000362.png|link=@linkclick,参数1,参数2,3>
    ]]
    say(actor,msg)
end

[[
    注意:如果需要传递参数到脚本接口，只需要在后面接 逗号 参数
    不支持老传奇传递参数的方式，lua里全部通过 @xxxx,1,2,3 这种方式传递参数
]]
function linkclick(actor,...)
    release_print("传入参数",...)
end
```
- **注意：一定小写**

