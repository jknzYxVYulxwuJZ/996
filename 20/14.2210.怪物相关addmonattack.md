### 添加自定义怪物攻击表现

`addmonattack`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数    | 类型      | 空   | 默认 | 注释                              |
| :------ | :-------- | :--- | :--- | :-------------------------------- |
| mon     | `object`  | 否   |      | 怪物对象                          |
| skillID | `integer` | 否   |      | 攻击表现id<br />对应cfg_monattack表 |

```lua
    addmonattack(mon,11)
```

