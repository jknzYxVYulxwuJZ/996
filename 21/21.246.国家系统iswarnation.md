### 判断国家之间是否宣战

`iswarnation`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.08.07新增接口&lt;/font&gt;**

| 参数       | 类型      | 空   | 默认 | 注释     |
| :--------- | :-------- | :--- | :--- | :------- |
| nationIDX1 | `integer` | 否   |      | 国家ID   |
| nationIDX2 | `integer` | 否   |      | 国家ID   |
| result     | `bool`    | 否   |      | 是否宣战 |
```lua
    local bool = iswarnation(countID_1,countID_2)
    LOGPrint("国家宣战",bool)
```

