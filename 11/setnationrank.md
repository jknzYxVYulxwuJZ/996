### 修改国家职位名称
`setnationrank`

| 参数    | 类型      | 空   | 默认 | 注释           |
| :------ | :-------- | :--- | :--- | :------------- |
| play    | `object`  | 否   |      | 玩家对象       |
| nIdx    | `integer` | 否   |      | 国家ID (1~100) |
| jobIdx  | `integer` | 否   |      | 职位编号       |
| jobName | `string`  | 否   |      | 职位名称       |
```lua
    setnationrank(actor,5,3,'汉奸')
```

