### 根据物品唯一ID获得物品对象

`getitembymakeindex`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |玩家对象 |
|makeindex     | `integer`      |否   |    |物品唯一ID |
|result     |`object`      |否   |    |物品对象 |
```
    会根据makeindex检索玩家装备和背包，返回对应的物品对象，如果检索不到，返回'0'
```

