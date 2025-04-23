### 把怪物设置成宝宝
`setmonmaster`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|mon     |`object`      |否   |    |   怪物对象 |
|player     |`object`      |否   |    |玩家对象 |

```lua
function main(self)
   local mon =  genmon(0,289,613,"黑野猪",10,1)
   setmonmaster(mon[1],self);
   say(self,"你获得了黑野猪宝宝")
end
```

