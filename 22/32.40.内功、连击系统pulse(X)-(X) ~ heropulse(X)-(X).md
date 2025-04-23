### 玩家/英雄穴位点击触发

`pulse(X)-(X)` ~ `heropulse(X)-(X)`

&gt; 第一个X为经络(0-4)，第二个X为穴位(1-5)

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |玩家对象 |
```lua
local function pulse(actor,param1,param2,...)
    release_print("穴位点击触发",getbaseinfo(actor,1),param1,param2,...)
end
for i = 0, 4 do
    for j = 1, 5 do
        _G[string.format("pulse%d-%d",i,j)] = function (actor,...)
            pulse(actor,i,j,...)
        end
    end
end
```

