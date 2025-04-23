### 清理自定义系统变量

`clearglobalcustvar`

| 参数 | 类型     | 空   | 默认 | 注释                |
| :--- | :------- | :--- | :--- | :------------------ |
| var  | `string` | 否   |      | 变量名, * -所有变量 |
```lua
    -- 多个变量用|分隔
    clearglobalcustvar("*")
    clearglobalcustvar("S变量1|S变量2")
```

