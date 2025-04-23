### 设置杀怪内功经验倍数

`killpulseexprate`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_23.12.07新增接口&lt;/font&gt;**

| 参数 | 类型      | 空   | 默认 | 注释                                                      |
| :--- | :-------- | :--- | :--- | :-------------------------------------------------------- |
| play | `object`  | 否   |      | 玩家对象                                                  |
| pro  | `integer` | 否   |      | 倍率<br />倍数除以100为真正的倍率(200为2倍经验，150为1.5倍) |
| time | `integer` | 否   |      | 有效时间(秒)                                              |
```lua
function main(actor)
    killpulseexprate(actor,1000 ,10)
    LOGPrint("您当前杀怪内功经验倍数为10倍，有效时间10秒。")
end
```

