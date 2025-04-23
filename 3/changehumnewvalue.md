### 修改人物临时属性（带有效期）
`changehumnewvalue`

| 参数   | 类型      | 空   | 默认 | 注释                          |
| :----- | :-------- | :--- | :--- | :---------------------------- |
| play   | `object`  | 否   |      | 玩家对象                      |
| nWhere | `integer` | 否   |      | 位置 对应cfg_att_score 属性ID |
| nValue | `integer` | 否   |      | 对应属性值                    |
| nTime  | `integer` | 否   |      | 有效时间，秒                  |

```lua
function main(self)
    changehumnewvalue(self,10,10,10)
end
```

