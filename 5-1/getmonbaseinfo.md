### 返回怪物基础信息
`getmonbaseinfo`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|idx     |`integer`      |否   |    |   怪物的IDX |
|id     |`integer`      |否   |    |id |
|result     |`variant`      |否   |    |返回值 |

- id取值：
1-怪物名称；
2-怪物名字颜色；
3-杀死怪物获得的经验值；

```lua
function main(self)
   local monname =  getmonbaseinfo(10001,1)
   say(self,monname)
end
```

