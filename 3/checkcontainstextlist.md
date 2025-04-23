### 检查字符串是否在指定文件中

- 注:包含检测,检测的字符串不需要完全相同,文件里的字符包含检测的字符,就会返回true

`checkcontainstextlist`

| 参数   | 类型      | 空   | 默认 | 注释                                                                                  |
| :----- | :-------- | :--- | :--- | :------------------------------------------------------------------------------------ |
| path   | `string`  | 否   |      | 文件路径                                                                              |
| str    | `string`  | 否   |      | 字符串                                                                                |
| model  | `integer` | 否   |      | 检测模式<br />0=列表中,是否包含被检测的字符<br />1=被检测的字符是否包含列表中的某一行内容 |
| result | `bool`    | 否   |      | true=在文件中<br />false=不在文件中                                                     |
```lua
local res1 = checkcontainstextlist('..\\QuestDiary\\abc.txt','ddd',0)
local res2 = checkcontainstextlist('..\\QuestDiary\\abc.txt','ddddddd',0)
local res3 = checkcontainstextlist('..\\QuestDiary\\abc.txt','dd',1)
local res4 = checkcontainstextlist('..\\QuestDiary\\abc.txt','ddddddd',1)
release_print('checkcontainstextlist',res1,res2,res3,res4)
```
