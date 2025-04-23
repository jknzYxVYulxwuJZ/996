### 获取物品基础属性
`getstditematt`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|itemid       |`integer`       |否   |    |   物品ID    |
|id       |`integer`       |否   |    |对应属性表的属性ID |
|result |`integer`         |是   |0    |   对应数值，不存在为0    |

 ```lua
function main(self)
    local item=linkbodyitem(self,0)
    if item then
        local itemid = getiteminfo(self,item,2)
        say(self, "关联物品0成功，唯一ID：" .. getiteminfo(self,item,1) .."\\物品名称："
        ..getstditeminfo(itemid,1)
        .."\\基础防御下限："..getstditematt(itemid,9)
        .."\\基础防御上限："..getstditematt(itemid,10)
        )
    else
        say(self, "关联物品0失败")
    end
end
```

