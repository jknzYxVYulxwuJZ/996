### 检测身上佩戴的装备

`checkitemw`

&gt; **&lt;font color="#808080" style="font-size: 13px;"&gt;引擎64_24.05.23新增接口&lt;/font&gt;**

| 参数      | 类型      | 空   | 默认 | 注释     |
| :-------- | :-------- | :--- | :--- | :------- |
| actor     | `object`  | 否   |      | 玩家对象 |
| item_name | `string`  | 否   |      | 装备名称 |
| item_num  | `integer` | 是   | 1    | 检测数量 |
| result    | `bool`    | 否   |      | 是否穿戴 |
```lua
    if not checkitemw(actor,"金手镯",2) then
        say(actor,"请先佩戴两个金手镯~")
        return
    end
```

