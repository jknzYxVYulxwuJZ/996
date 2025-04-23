### 添加buff

`addbuff`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|base     |`object`        |否   |    |   玩家、怪物对象    |
|buffid       |`integer`       |否   |    |   buff id，10000以后   |
|time     |`integer`       |是   |    |   时间,对应buff表里维护的单位   |
|OverLap      |`integer`       |是   |    |  叠加层数，默认1    |
|objOwner     |`object`        |是   |    |  施放者    |
|Abil     |`table`     |是   |    |  属性表 {[1]=200, [4]=20}，属性id=值   |
|result       |`bool`      |否   |    |  是否添加成功    |

