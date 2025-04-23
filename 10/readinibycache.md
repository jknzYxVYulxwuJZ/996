### 读取Ini文件中的字段值（带Cache）
`readinibycache`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|filename     |`string`        |否   |    |  文件名   |
|section      |`string`        |否   |    |  配置项区   |
|item     |`string`        |否   |    |  配置项   |
|result       |`string`        |否   |    |  配置项值   |
```lua
    local str = readinibycache("QuestDiary/test.ini","Setup","temp1")
    release_print("str",str)
```
