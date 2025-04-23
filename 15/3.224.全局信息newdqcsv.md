### 读取表里面的第几行第几列内容(0行0列开始)
`newdqcsv`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|filename     |`string`        |否   |    |  文件名   |
|row      |`int`       |否   |    |  行数   |
|col      |`int`       |否   |    |  列数   |
|result       |`string`        |否   |    |  表内数据   |
```lua
    local str = newdqcsv("QuestDiary\\test.csv",4,0)
    release_print("第4行,第0列",str)
```

