### 玩家/英雄修炼经络触发

`pulselvup(X)` ~ `heropulselvup(X)`

&gt; X为经络(0-4)

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |玩家对象 |
```lua
local function pulselvup(actor,param1,...)
    release_print("穴位点击触发",getbaseinfo(actor,1),param1,...)
end
for i = 0, 4 do
    _G[string.format("pulselvup%d",i)] = function (actor,...)
        pulselvup(actor,i,...)
    end
end
```

## 接口

