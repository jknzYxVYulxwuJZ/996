#### 拍卖购买物品触发

`buypaimaiitem`

| 参数          | 类型      | 空   | 默认 | 注释       |
| :------------ | :-------- | :--- | :--- | :--------- |
| actor         | `object`  | 否   |      | 玩家对象   |
| itemIdx       | `integer` | 否   |      | 物品id     |
| itemMakeIndex | `integer` | 否   |      | 物品唯一id |
| moneyType     | `integer` | 否   |      | 货币类型   |
| price         | `integer` | 否   |      | 价格       |

```lua
function buypaimaiitem(actor,itemIdx,itemMakeIndex,moneyType,price)
    if getbaseinfo(actor,6) &lt; 50 then
        say(actor,"禁止购买物品")
        allowpaimai(actor,1)
        [[23.0830前引擎需要调用TXT命令打断,callscriptex(actor,"allowpaimai","1")]]
        return
    end
end

```

