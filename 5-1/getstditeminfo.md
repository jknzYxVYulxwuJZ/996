### 获取物品基础信息
`getstditeminfo`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|itemid/itemName      |`integer`/`string`      |否   |    |   物品ID/物品名称    |
|id       |`integer`       |否   | 13:物品颜色<br />引擎64_23.0628新增   |0:idx <br /> 1:名称 <br />2:StdMode<br />3:Shape<br />4:重量<br />5:AniCount <br />6:最大持久 <br />7:叠加数量<br />8:价格（price）<br />9:使用条件 <br />10:使用等级<br />11:自定义常量(29列)<br />12:自定义常量(30列)<br />13:道具颜色 |
|result |`integer`         |是   |0    |   对应数值，不存在为0    |

