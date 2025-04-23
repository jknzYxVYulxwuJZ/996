#### 添加-setontimerex
`setontimerex`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|id     |`integer`      |否   |    |   定时器ID |
|tick |`integer`  |否 | |执行间隔，秒|
```lua
        setontimerex(23, 5)

        --触发函数为ontimerex 拼接 定时器id
        function ontimerex23()
        end
```
