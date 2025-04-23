### 获取当前表格最大行数、和获取表格最大列数
`gethlcsv`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|filename     |`string`        |否   |    |  文件名   |
|type     |`int`       |否   |    |  读取目标：0-行数，1-列数   |
```lua
    local w = gethlcsv("QuestDiary\\test.csv",0)
    local h = gethlcsv("QuestDiary\\test.csv",1)
    release_print("行数",w)
    release_print("列数",h)
```
