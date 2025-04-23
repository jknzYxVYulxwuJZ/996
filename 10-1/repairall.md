### 修复所有装备
`repairall`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |  玩家对象 |

```lua
    [[
        需要在npc脚本中使用,且文件头需设置itemstype表储存需要修复的装备位置
        Mir200\Envir\Market_Def\第一大陆\装备修复-3.lua
    ]]
    itemstype = {1,2,3,4,5,6,7,8,9,10}
    function main(actor)
        local msg =[[&lt;设置持久/@chijiu&gt;\&lt;一键修复/@xiufu&gt;]]
        say(actor,msg)
    end
    function chijiu(actor)
        local itemobj = linkbodyitem(actor,1)
        local itemMakeId = getiteminfo(actor,itemobj,1)
        setdura(actor,itemMakeId,"=",2000)
    end
    function xiufu(actor)
        repairall(actor)
    end
```

