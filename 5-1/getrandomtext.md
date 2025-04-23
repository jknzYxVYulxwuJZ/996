### 从文件中随机获取一行字符串

`getrandomtext`

| 参数 | 类型     | 空   | 默认 | 注释           |
| :--- | :------- | :--- | :--- | :------------- |
| path | `string` | 否   |      | 文件路径       |
| line | `integer` | 是   |  0    | 指定行(0~1000)<br />传入-1随机取某一行的字符串 |
```lua
local str = getrandomtext('..\\QuestDiary\\abc.txt',-1)
release_print('getrandomtext',str)
```

