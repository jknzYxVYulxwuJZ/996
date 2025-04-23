### 取字符串在列表中的下标

`getstringpos`

| 参数   | 类型      | 空   | 默认 | 注释                          |
| :----- | :-------- | :--- | :--- | :---------------------------- |
| path   | `string`  | 否   |      | 文件路径                      |
| str    | `string`  | 否   |      | 字符串                        |
| result | `integer` | 否   |      | 字符串所在行<br />未找到返回9999999 |
```lua
local pos = getstringpos('..\\QuestDiary\\abc.txt','aaa')
release_print('getstringpos',type(pos),pos)
```

