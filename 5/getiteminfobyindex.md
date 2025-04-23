### 获取背包物品数量

`getbagitemcount`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|itemname     |`string`      |否   |    |  物品名称 |
|model     |`string`      |否   |  引擎64_23.10.24新增  | 物品绑定状态<br />0=忽略;<br />1=非绑定;<br />2=绑定; |
|result     |`integer`      |否   |    |   返回值，对应物品的数量 |
```lua
    local itemNum = getbagitemcount(actor,"木剑")
    release_print("itemNum",itemNum)
```

## 根据索引返回背包物品信息

&gt; 删物品需判断是否成功

`getiteminfobyindex`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|index    |`integer`       |否   |    |    索引号,0开始   |
|result       |`object`        |否   |    |  物品对象  |

