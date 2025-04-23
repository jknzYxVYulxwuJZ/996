### 清理自定义行会变量

`clearguildcustvar`

| 参数      | 类型     | 空   | 默认 | 注释                       |
| :-------- | :------- | :--- | :--- | :------------------------- |
| guildName | `string` | 否   |      | 行会名称, <br> * -所有行会 |
| var       | `string` | 否   |      | 变量名, <br> * -所有变量   |
```lua
    -- 多个行会用|分隔，多个变量用|分隔
    clearguildcustvar("*","*")
    clearguildcustvar("行会名称","S变量1|S变量2")
```
