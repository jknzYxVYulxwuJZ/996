### 获取buff信息

`getbuffinfo`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|base     |`object`        |否   |    |   玩家、怪物对象    |
|buffid       |`integer`       |否   |    |   buff id   |
|type     |`integer`       |否   |  类型3/4新增于<br />引擎64_23.10.24  | 1=叠加层数 <br />2=剩余时间(单位跟配置一致)<br />3=获取施法者对象(对象离线返回nil)<br />4=获取额外属性   |
|result       |`integer`       |否   |    |   返回值    |

