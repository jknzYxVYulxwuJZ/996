### 检测范围内怪物数量
`checkrangemoncount`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|mapid     |`string`      |否   |    |   地图Id |
|monName     |`string`      |否   |    |怪物名，为空 or * 为检测所有怪 |
|nx     |`integer`      |否   |    |坐标X |
|nx     |`integer`      |否   |    |坐标Y |
|nRange     |`integer`      |否   |    |范围 |
|result     |`integer`      |否   |    |返回值，数量 |

```lua
function main(self)
   say(self,'该范围有'..checkrangemoncount('0','',285,612,10)..'只怪')
end
```
