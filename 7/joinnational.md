### 加入/退出国家
`joinnational`

&gt; 异步接口

| 参数   | 类型      | 空   | 默认 | 注释                         |
| :----- | :-------- | :--- | :--- | :--------------------------- |
| play   | `object`  | 否   |      | 玩家对象                     |
| nIdx   | `integer` | 否   |      | 国家ID (1~100),填0退出国家   |
| jobIdx | `integer` | 否   |      | 职位编号（0-9 不填 默认为0） |
```lua
    joinnational(actor,5,9) --加入国家
    joinnational(actor,0)   --退出国家
```

