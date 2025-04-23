### 检查字符串是否在指定文件中

- 注:不区分大小写

`checktextlist`

| 参数   | 类型     | 空   | 默认 | 注释                              |
| :----- | :------- | :--- | :--- | :-------------------------------- |
| path   | `string` | 否   |      | 文件路径                          |
| str    | `string` | 否   |      | 字符串                            |
| result | `bool`   | 否   |      | true=在文件中<br />false=不在文件中 |
```lua
local res1 = checktextlist('..\\QuestDiary\\abc.txt','ccc')
release_print('checktextlist',res1,res2)
```

