### 设置人物货币
`changemoney`

| 参数   | 类型      | 空   | 默认 | 注释                        |
| :----- | :-------- | :--- | :--- | :-------------------------- |
| play   | `object`  | 否   |      | 玩家对象                    |
| id     | `integer` | 否   |      | 货币ID（1-100）             |
| opt    | `char`    | 否   |      | 操作符 + - =                |
| count  | `integer` | 否   |      | 数量                        |
| msg    | `string`  | 否   |      | 备注内容                    |
| send   | `bool`    | 否   |      | 是否推送到客户端，true-更新 |
| result | `bool`    | 否   |      | 是否成功                    |

