#### 拍卖行重新上架前触发

`canrepaimaiitem`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数          | 类型      | 空   | 默认 | 注释       |
| :------------ | :-------- | :--- | :--- | :--------- |
| actor         | `object`  | 否   |      | 玩家对象   |
| itemIdx       | `integer` | 否   |      | 物品id     |
| itemMakeIndex | `integer` | 否   |      | 物品唯一id |
| moneyType     | `integer` | 否   |      | 货币类型   |
| price1        | `integer` | 否   |      | 竞拍价     |
| price2        | `integer` | 否   |      | 一口价     |

```lua
function canrepaimaiitem(actor,itemIdx,itemMakeIndex,moneyType,price1,price2)
    if price2 &lt; 100 then
        say(actor,"一口价过低禁止上架!")
        allowpaimai(actor,1)
        return
    end
end

```

