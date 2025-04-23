### 设置物品绑定状态

`setitemstate`

| 参数  | 类型      | 空   | 默认 | 注释                           |
| :---- | :-------- | :--- | :--- | :----------------------------- |
| item  | `object`  | 否   |      | 物品对象                       |
| bind  | `integer` | 否   |      | 绑定类型(0-8,21)               |
| state | `integer` | 否   |      | 绑定状态<br />0=不绑定<br />1=绑定 |
```lua
local config = {
    [0] = "禁止扔",
    [1] = "禁止交易",
    [2] = "禁止存",
    [3] = "禁止修",
    [4] = "禁止出售",
    [5] = "禁止爆出",
    [6] = "丢弃消失",
    [7] = "死亡必爆(死亡爆出来后，该属性就会删除，在捡起来戴上，就没有死亡必爆了)",
    [8] = "禁止摆摊或上架拍卖行",
    [21] = "爆出消失[引擎64_24.03.14新增]",
}
-- 捡取任意物品前触发
function pickupitemfrontex(actor, itemobj)
    for i, v in pairs(config) do
        setitemstate(itemobj,i,1)
        local state1 = getiteminfo(actor,itemobj,6)
        local state2 = checkitemstate(itemobj,i)
        release_print("状态:",i,v,state1,state2)
    end
end
```

