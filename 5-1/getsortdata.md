###**排行榜配置可根据自定义变量进行排序(有排行榜的版本必须配置)**

自定义排行榜过滤文件,将玩家角色ID"<$USERID>"添加到该文本后,玩家将不参与排行统计

过滤文件路径:`Mir200\Envir\QuestDiary\SortFilter.txt`

cfg_game_data.xls配置字段：`SortConfig` `参数1#参数2#参数3|参数1#参数2#参数3|参数1#参数2#参数3`

`参数1`：面板ID---自定义ID，用于打开对应面板
`参数2`：职业------0战士，1法师，2道士，3全部主号 10英雄战士，11英雄法师，12英雄道士, 13英雄全部
`参数3`：类型------1转生，2等级，3变量#自定义变量名

`M2--功能设置--其他设置-排行榜设置`

------------

> [**自定义排行榜示例下载**](http://engine-doc.996m2.com/server/index.php?s=/api/attachment/visitFile&sign=7ae846b6b05d868125d21d2e08799a29 "[QFunction-0 - 自定义排行榜.zip")

## 自定义排行榜刷新触发

`inisort`

| 参数   | 类型     | 空   | 默认 | 注释     |
| :----- | :------- | :--- | :--- | :------- |
| sysobj | `string` | 否   |      | 系统对象 |

## 自定义排行榜切换玩家和英雄的页签触发

`clicksortbutton`

| 参数   | 类型     | 空   | 默认 | 注释                               |
| :----- | :------- | :--- | :--- | :--------------------------------- |
| actor  | `string` | 否   |      | 玩家对象                           |
| ishero | `number` | 否   |      | 0=打开玩家页签；<br>1=打开英雄页签 |

## 自定义排行榜点击排名触发

`clicksortno`

| 参数    | 类型     | 空   | 默认 | 注释       |
| :------ | :------- | :--- | :--- | :--------- |
| actor   | `string` | 否   |      | 玩家对象   |
| ranking | `number` | 否   |      | 排行榜名次 

## 获取自定义排行榜缓存数据

`getsortdata`

> **<font color="#808080" style="font-size: 13px;">引擎64_24.05.23新增接口</font>**

| 参数    | 类型     | 空   | 默认 | 注释                   |
| :------ | :------- | :--- | :--- | :--------------------- |
| rankidx | `object` | 否   |      | 自定义排行榜页签       |
| result  | `string` | 否   |      | 排行榜数据<br>json格式 |

```lua
    local rank_index = 1
    local rank_list = json2tbl(getsortdata(rank_index))
```
