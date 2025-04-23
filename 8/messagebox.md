### 弹出窗口消息
`messagebox`

| 参数   | 类型     | 空   | 默认 | 注释             |
| :----- | :------- | :--- | :--- | :--------------- |
| player | `object` | 否   |      | 玩家对象         |
| info   | `string` | 否   |      | 弹出内容         |
| flag1  | `string` | 否   |      | 确定后跳转的接口 |
| flag2  | `string` | 否   |      | 取消后跳转的接口 |
```lua
messagebox(actor,"系统消息\\待填写的文本..","@func_ok,1,2,3","@func_no,4,5,6")

function func_ok(actor,...)
    release_print("func_ok",...)
end

function func_no(actor,...)
    release_print("func_no",...)
end
```

