### 遍历宠物(宝宝)列表
`getslavebyindex`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|nIndex     |`integer`      |否   |    |   索引(0开始) |
|result     |`object`      |否   |    |   怪物对象 |

```lua
function main(actor)
    local ncount=getbaseinfo(actor,38)
    for i = 0 ,ncount-1 do
        local mon = getslavebyindex(actor, i)
        if mon and isnotnull(mon) then
            setbaseinfo(mon,20,getbaseinfo(mon,20)+10)
        end
    end
    say(actor,'你的所有宝宝增加10点攻击')
end
```

