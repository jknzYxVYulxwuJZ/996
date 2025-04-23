### 取字符串在csv表格中的行号
`getgjcsv`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|filename     |`string`        |否   |    |  文件名   |
|str      |`string`        |否   |    |  字符串   |
|rowlimit     |`string`        |否   |    |  行数限制，格式：开始行号-结束行号   |
|col      |`int`       |否   |    |  查找的列数   |
|findtype     |`int`       |否   |    |  查找类型：<br />0-在开始哪行;<br /> 1-在最后哪行;    |

```lua
    local param = getgjcsv("QuestDiary\\test.csv","2","0-5",0,0)
    release_print("字符串'2'在0列开始第"..param.."行")
```

------------

