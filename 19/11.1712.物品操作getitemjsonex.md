### 设置物品特效

`setitemeffect`

| 参数        | 类型      | 空   | 默认                | 注释                      |
| :---------- | :-------- | :--- | :------------------ | :------------------------ |
| play        | `object`  | 否   |                     | 玩家对象                  |
| itemPos     | `integer` | 否   |                     | 装备位置(-2操作物品对象)  |
| bageffectid | `integer` | 否   |                     | 背包特效编号              |
| ineffectid  | `integer` | 否   |                     | 内观特效编号              |
| order1      | `integer` | 否   |                     | 背包特效层级<br />0=前;1=后 |
| order2      | `integer` | 否   |                     | 内观特效层级<br />0=前;1=后 |
| item        | `object`  | 否   | 引擎64_23.08.30新增 | 物品对象                  |
```lua
--根据装备位设置特效
setitemeffect(actor,1,5111,6063,1,1)

--根据物品对象设置特效
setitemeffect(actor,-2,6307,6063,nil,nil,itemobj)
```

------------

## 根据物品获取Json

`getitemjson`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|item     |`object`      |否   |    |  物品对象 |
|result     |`string`        |否   |    |  json字符串   |

```json
{
    "MakeIndex":xxxx,
    "Idx":xxxx,
    "Name":xxxx,
    "Dura":xxxx,
    "DuraMax":xxxx,
    "Overlap":xxxx,
    "AddValue0":xxxx,
    "AddValue1":xxxx,
    "ExAbil":xxxx
}
```
```lua
    local json = getitemjson(item)
```

## 根据json字符串给物品
`giveitembyjson`

| 参数   | 类型     | 空   | 默认                | 注释           |
| :----- | :------- | :--- | :------------------ | :------------- |
| actor  | `object` | 否   |                     | 玩家对象       |
| json   | `string` | 否   |                     | json字符串     |
| desc   | `string` | 是   | 引擎64_24.05.23新增 | 描述           |
| result | `object` | 否   |                     | 生成的物品对象 |

```json
{
    "MakeIndex":xxxx,
    "Idx":xxxx,
    "Name":xxxx,
    "Dura":xxxx,
    "DuraMax":xxxx,
    "Overlap":xxxx,
    "AddValue0":xxxx,
    "AddValue1":xxxx,
    "ExAbil":xxxx
}
*注 : 根据json字符串给的物品，将会生成新的MakeIndex
```

## 根据物品获取前端显示的Json

`getitemjsonex`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.12.07新增接口&lt;/font&gt;**

| 参数   | 类型     | 空   | 默认 | 注释       |
| :----- | :------- | :--- | :--- | :--------- |
| item   | `object` | 否   |      | 物品对象   |
| result | `string` | 否   |      | json字符串 |
```lua
function main(actor)
    local itemobj = linkbodyitem(actor,1)
    local itemjson = getitemjsonex(itemobj)
    str = [[&lt;ItemShow|x=0.0|y=0.0|width=70|height=70|itemdata=]]..itemjson..[[|showtips=1|bgtype=1|color=250&gt;]]
    say(actor,itemobj)
end
```

------------

