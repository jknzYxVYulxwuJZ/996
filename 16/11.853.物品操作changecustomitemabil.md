### 绑定自定义装备属性
`changecustomitemabil`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |   玩家对象 |
|item     |`object`        |否   |    |  物品对象   |
|attrindex  |`integer`         |是   |0    |  属性位置(0~9)每个装备可以自定义10个属性    |
|bindindex  |`integer`         |是   |0    |  绑定类型(0~4)  |
|bindvalue  |`integer`         |是   |0    |  绑定的值    |
|group  |`integer`         |是   |0    |  显示分类位置<br />(0~5 ;为空默认为0)    |

```
    绑定类型(0~4):
    0=标识该属性绑定的颜色值默认读取(属性表:cfg_custpro_caption.xls)里面的颜色
    1=表示该绑定属性表(属性ID:cfg_att_score.xls的属性ID),必须绑定，否则该属性无效，游戏也不会显示
    2=标示该属性绑定自定义属性表:cfg_custpro_caption.xls里面的属性ID
    3=表示该属性是否是百分比属性(0,1) 0不是百分比 1是百分比
    4=属性显示位置(0~9) 如果一行有多个属性,这里位置就写同一行
    
    绑定的值:
    参数4(绑定类型)=0时 绑定属性颜色(0~255) 默认读取(属性表:cfg_custpro_caption.xls)里面的颜色
    参数4(绑定类型)=1时 绑定属性表:cfg_att_score.xls里面的属性ID
    参数4(绑定类型)=2时 绑定自定义属性表:cfg_custpro_caption.xls里面的属性ID
    参数4(绑定类型)=3时 绑定的值(0~1)
    参数4(绑定类型)=4时 显示位置(0~9)
```
```lua
    local itemobj = linkbodyitem(actor,1)
    local itemidx = getiteminfo(actor,itemobj,2)
    local itemName = getstditeminfo(itemidx,1)
    local weizhi = 0
    local attrIndex = 4
    local attrValue = 100
    release_print(itemName,"修改属性",attrIndex .."+" .. attrValue)
    changecustomitemtext(actor, itemobj, "[自定义属性测试]：", 0)
    changecustomitemtextcolor(actor, itemobj, 253, 0)
    changecustomitemabil(actor,itemobj,weizhi,0,214,0)
    changecustomitemabil(actor,itemobj,weizhi,1,attrIndex,0)
    -- changecustomitemabil(actor,itemobj,weizhi,2,1,0)
    -- changecustomitemabil(actor,itemobj,weizhi,3,0,0)
    changecustomitemabil(actor,itemobj,weizhi,4,weizhi,0)
    changecustomitemvalue(actor,itemobj,weizhi,"+",attrValue,0)
    refreshitem(actor,itemobj)
```

