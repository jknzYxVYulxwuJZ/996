### 杀怪1
`killmonsters`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|mapid     |`string`      |否   |    |   地图id |
|monname     |`string`      |否   |    |怪物全名，空 或者 * 杀死全部 |
|count     |`integer`      |否   |    |   数量，0所有 |
|drop     |`bool`      |否   |    |   是否掉落物品，true掉落 |

```lua
function main(self)
    killmonsters(0,"*",5,true)
end
```

