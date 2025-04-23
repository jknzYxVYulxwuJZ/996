### 写入指定文本文件

`addtextlist`

| 参数 | 类型     | 空   | 默认 | 注释              |
| :--- | :------- | :--- | :--- | :---------------- |
| path | `string` | 否   |      | 文件路径          |
| str  | `string` | 否   |      | 写入文本          |
| line | `integer` | 否   |      | 写入行数(0~65535) |
```lua
addtextlist('..\\QuestDiary\\abc.txt','aaa',0)
addtextlist('..\\QuestDiary\\abc.txt','bbb',1)
addtextlist('..\\QuestDiary\\abc.txt','ccc',2)
addtextlist('..\\QuestDiary\\abc.txt','ddd',3)
addtextlist('..\\QuestDiary\\abc.txt','eee',4)
addtextlist('..\\QuestDiary\\abc.txt','aaa|bbb|ccc|ddd|eee',5)
```

