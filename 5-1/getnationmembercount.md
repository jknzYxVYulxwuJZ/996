### 获取国家人数

`getnationmembercount`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.08.07新增接口&lt;/font&gt;**

| 参数      | 类型      | 空   | 默认 | 注释     |
| :-------- | :-------- | :--- | :--- | :------- |
| nationIDX | `integer` | 否   |      | 国家ID   |
| result    | `integer` | 否   |      | 国家人数 |
```lua
    local count = getnationmembercount(countID_1)
    LOGPrint("国家人数",count)
```
