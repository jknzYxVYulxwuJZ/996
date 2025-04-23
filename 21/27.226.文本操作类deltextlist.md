### 删除文本文件的内容

`deltextlist`

| 参数  | 类型      | 空   | 默认 | 注释                                                        |
| :---- | :-------- | :--- | :--- | :---------------------------------------------------------- |
| path  | `string`  | 否   |      | 文件路径                                                    |
| line  | `integer`  | 否   |      | 指定行                                                      |
| model | `integer` | 否   |      | 删除模式<br />0=删除行<br />1=清空行<br />2=删除随机行(参数2失效) |
```lua
--删除第0行
deltextlist('..\\QuestDiary\\abc.txt',1,0)
--清空第0行
deltextlist('..\\QuestDiary\\abc.txt',1,1)
--随机删除一行
deltextlist('..\\QuestDiary\\abc.txt',nil,2)
```

