### 是否满足指定条件购买（canbuyshopitem触发中使用）
`notallowbuy`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|canbuy     |`integer`      |否   |    | 1-不允许购买，0-允许购买 |

## 敏感词汇检测
`exisitssensitiveword` 需要维护Envir目录下的 SensitiveWord.txt。  

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|str     |`string`      |否   |    |   要检测的文本 |
|result1     |`bool`    |否   |    | true：有敏感词 |
|result2     |`string`  |否   |    |   敏感词 |

