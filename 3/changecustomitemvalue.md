### 修改自定义属性值
`changecustomitemvalue`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|item     |`object`        |否   |    |  物品对象   |
|attrindex  |`integer`         |是   |0    |  属性位置(0~9)每个装备可以自定义10个属性    |
|operate  |`string`        |是   |    |  操作符：+、-、=  |
|value  |`integer`         |是   |0    |  属性值    |
|group  |`integer`         |是   |0    |  显示分类位置<br />(0~5 ;为空默认为0)    |

