### 获取文本文件指定行的内容

`getliststring`

| 参数   | 类型     | 空   | 默认 | 注释     |
| :----- | :------- | :--- | :--- | :------- |
| path   | `string` | 否   |      | 文件路径 |
| line   | `integer` | 否   |      | 指定行   |
| result | `string` | 否   |      | 字符串 |
| result | `string` | 否   |      | 返回值2<br />当有内容中存在`:`时,会将`:`号后的字符分割返回 |
```lua
    abc.txt中的文本内容,当行内有`:`号时,
    [[
        aaa:99999
        bbbvvv
    ]]
    local line = 0
    local res1,res2 = getliststring('..\\QuestDiary\\abc.txt',line)
    release_print('getliststring',line,res1,res2)

    -- M2打印结果
    `getliststring,0,aaa,99999`

    local line = 1
    local res1,res2 = getliststring('..\\QuestDiary\\abc.txt',line)
    release_print('getliststring',line,res1,res2)

    -- M2打印结果
    `getliststring,1,bbbvvv,`
```

