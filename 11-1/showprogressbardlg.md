### 采集挖矿等进度条操作

`showprogressbardlg`

| 参数    | 类型      | 空   | 默认 | 注释                                 |
| :------ | :-------- | :--- | :--- | :----------------------------------- |
| play    | `object`  | 否   |      | 玩家对象                             |
| time    | `integer` | 否   |      | 进度条时间，秒                       |
| succ    | `string`  | 否   |      | 成功后跳转的函数                     |
| msg     | `string`  | 否   |      | 提示消息                             |
| canstop | `integer` | 否   |      | 能否中断<br />0-不可中断<br />1-可以中断 |
| fail    | `string`  | 否   |      | 中断触发的函数                       |
```lua
showprogressbardlg(actor,5,"@func_1","进度条测试..", 1,"@func_2")

[[注:跳转函数不能附带参数]]
function func_1(actor)
    release_print("func_1",getbaseinfo(actor,1))
end

function func_2(actor)
    release_print("func_2",getbaseinfo(actor,1))
end
```

