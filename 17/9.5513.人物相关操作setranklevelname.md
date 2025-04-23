### 完美封号系统
`setranklevelname`

| 参数      | 类型     | 空   | 默认 | 注释                     |
| :-------- | :------- | :--- | :--- | :----------------------- |
| play      | `object` | 否   |      | 玩家对象                 |
| levelname | `string` | 否   |      | 称号文本，和名字一起显示 |
```lua
--显示在名字上方
setranklevelname(actor,"%s\\[击杀xx人]")

--显示在名字后方
setranklevelname(actor,"%s[击杀xx人]")
```

## 攻击模式

