### 修改物品持久度
`setdura`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|itemmakeid       |`integer`       |否   |    |  唯一ID   |
|char  |`string`      |否   |    |  操作符(+ - =)    |
|dura  |`integer`      |否   |    |  持久度    |
```lua
    setdura(actor,itemmakeid,"=",1000)
```

