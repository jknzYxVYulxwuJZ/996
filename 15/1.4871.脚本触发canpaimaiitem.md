#### 拍卖行上架触发

`canpaimaiitem`

| 参数          | 类型      | 空   | 默认                | 注释       |
| :------------ | :-------- | :--- | :------------------ | :--------- |
| actor         | `object`  | 否   |                     | 玩家对象   |
| itemIdx       | `integer` | 否   |                     | 物品id     |
| itemMakeIndex | `integer` | 否   |                     | 物品唯一id |
| moneyType     | `integer` | 否   |                     | 货币类型   |
| price1        | `integer` | 否   |                     | 竞拍价     |
| price2        | `integer` | 否   | 引擎64_24.05.23新增 | 一口价     |

```lua
function canpaimaiitem(actor,itemIdx,itemMakeIndex,moneyType,price1,price2)
    if getbaseinfo(actor,6) &lt; 50 then
        say(actor,"禁止上架物品")
        allowpaimai(actor,1)
        [[23.0830前引擎需要调用TXT命令打断,callscriptex(actor,"allowpaimai","1")]]
        return
    end
end

```

