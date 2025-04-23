### 删除延迟

`cleardelaygoto`

| 参数 | 类型     | 空   | 默认                | 注释                                 |
| :--- | :------- | :--- | :------------------ | :----------------------------------- |
| play | `object` | 否   |                     | 玩家对象                             |
| func | `string` | 否   | 引擎64_23.08.30新增 | 需要删除的延时函数<br />不填为清除全部 |
```lua
delaygoto(actor,1000,"test_jump1",0)
cleardelaygoto(actor,"test_jump1")

delaygoto(actor,1000,"test_jump2,1,2,3",0)
cleardelaygoto(actor,"test_jump2,1,2,3")
```

