### 获取装备钻石镶嵌情况
`getsocketableitem`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|item     |`object`        |否   |    |  装备对象   |
|result   |`string`        |否   |    |  开孔相关，json字符串，支持0~9共10个孔    |
```json
socketableitem 镶嵌宝石，传入json
getsocketableitem 返回镶嵌宝石的json
{
    socket0: 20333,  //第0个孔位置，20333-对应宝石的Index，
    socket1: 0,  //第1个孔位置，0-未镶嵌宝石
    socket2: 0,
    socket3: -1,  //第3个孔位置，-1-未打孔
    socket4: -1,
    socket5: -1,
    socket6: 0,
    socket7: -1,
    socket8: -1,
    socket9: -1
}

```
