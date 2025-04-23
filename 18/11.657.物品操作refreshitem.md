### 设置-setitemaddvalue
`setitemaddvalue`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|item     |`object`        |否   |    |   物品对象   |
|type     |`integer`       |否   |    |[1,2,3] |
|position     |`integer`       |否   |    |当type=1,取值范围[0..49] <br /> type=2,取值范围[0..19]|
|value |`integer`      |否   |    |   设置物品对应位置值    |

## 刷新物品信息到前端
`refreshitem`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|item     |`object`        |否   |    |  物品对象   |

```lua
function main(self)
    local item = linkbodyitem(self, 0)
    if item then
        local itemid = getiteminfo(self, item, 2)
        local str
        str = ""
        for i = 0, 49 do
            str = str .. "," .. getitemaddvalue(self, item, 1, i)
        end
        str = str .. "\\"
        for i = 0, 19 do
            str = str .. "," .. getitemaddvalue(self, item, 2, i)
        end
        say(self, str);
        setitemaddvalue(self, item, 1, 1, math.random(100));
        refreshitem(self, item);
        recalcabilitys(self)
    else
        say(self, "关联物品0失败")
    end
end
```
## 自定义属性
