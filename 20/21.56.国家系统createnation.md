### 创建国家
`createnation`

| 参数   | 类型      | 空   | 默认 | 注释           |
| :----- | :-------- | :--- | :--- | :------------- |
| play   | `object`  | 否   |      | 玩家对象       |
| nIdx   | `integer` | 否   |      | 国家ID (1~100) |
| name   | `string`  | 否   |      | 国家名称       |
| maxNum | `integer` | 否   |      | 限制人数       |
```lua
    createnation(actor,5,'华夏',100)
```
