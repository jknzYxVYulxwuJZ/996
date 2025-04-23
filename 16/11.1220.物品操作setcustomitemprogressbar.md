### 设置自定义进度条参数
`setcustomitemprogressbar`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|item     |`object`        |否   |    |  装备对象   |
|index  |`integer`         |否   |    |   装备精度条索引（0~2）    |
|json  |`string`       |否   |    |   进度条内容，json字符串    |
```lua
    [[
        // json格式，json中各项参数均可以为空：
        {
            open:1,  //0-关闭，1-打开
            show:1,  //0-不显示数值，1-百分比，2-数字
            name:"锻造",  //进度条文本
            color:3,  //进度条颜色，0~255
            imgcount:1,  //图片张数，填1即可
            cur:0,  //当前值
            max:100,  //最大值
            level:0  //级别(0~65535)
        }
    ]]
    local itemobj = linkbodyitem(actor,1)
    local tbl = {
        ["open"] = 1,
        ["show"] = 2,
        ["name"] = "经验值",
        ["color"] = 253,
        ["imgcount"] = 1,
        ["cur"] = 2500,
        ["max"] = 5000,
        ["level"] = 0,
    }
    setcustomitemprogressbar(actor,itemobj,0,tbl2json(tbl))
    refreshitem(actor,itemobj)
```

