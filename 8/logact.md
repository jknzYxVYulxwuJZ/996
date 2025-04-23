### 自定义日志

- 说明: 配置自定义日志对应后台查看

`logact`

| 参数    | 类型      | 空   | 默认 | 注释                         |
| :------ | :-------- | :--- | :--- | :--------------------------- |
| play    | `object`  | 否   |      | 玩家对象                     |
| logAct  | `integer` | 否   |      | 日志ID<br />大于等于10000以上  |
| loginfo | `string`  | 否   |      | 日志内容<br />支持变量,常量等  |
| nParam1 | `integer` | 否   |      | 整数型(可空)<br />最大支持21亿 |
| nParam2 | `integer` | 否   |      | 整数型(可空)<br />最大支持21亿 |
| nParam3 | `integer` | 否   |      | 整数型(可空)<br />最大支持21亿 |
| nParam4 | `integer` | 否   |      | 整数型(可空)<br />最大支持21亿 |
| nParam5 | `integer` | 否   |      | 整数型(可空)<br />最大支持21亿 |

```lua
logact(actor,10001,"玩家：&lt;$username&gt;通过日志测试扣除100元宝获得屠龙*1",1,2,3,4,5)
```
![后台上传表格格式](http://engine-doc.996m2.com/server/index.php?s=/api/attachment/visitFile&amp;sign=41626a76cfe8f49ab0a80f948b891ea8)

