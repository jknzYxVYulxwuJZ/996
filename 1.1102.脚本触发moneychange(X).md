### 货币改变触发

`moneychange(X)`

&gt; X=货币道具表idx

| 参数  | 类型     | 空   | 默认 | 注释     |
| :---- | :------- | :--- | :--- | :------- |
| actor | `object` | 否   |      | 玩家对象 |

```lua
for moneyIdx = 1, 100 do
    _G["moneychange"..moneyIdx] = function (actor)
        local formernum = getconst(actor, "&lt;$OLDMONEY&gt;")
        local curnum = querymoney(actor, moneyIdx)
        local name = getstditeminfo(moneyIdx, 1)
        release_print("货币【"..name.."】改变：", moneyIdx, curnum, formernum)
    end
end

```

