### 获取文本文件指定行的内容[根据符号分割]

`getliststringex`

| 参数   | 类型     | 空   | 默认 | 注释     |
| :----- | :------- | :--- | :--- | :------- |
| path   | `string` | 否   |      | 文件路径 |
| line   | `integer` | 否   |      | 指定行   |
| symbol | `string` | 否   |      | 符号     |
```lua
local tbl = getliststringex('..\\QuestDiary\\abc.txt',5,'|')
for i,v in ipairs(tbl or {}) do
    release_print("文本",i,v)
end
```

