### 初始化自定义变量

`inisysvar`

| 参数      | 类型     | 空   | 默认 | 注释                     |
| :-------- | :------- | :--- | :--- | :----------------------- |
| varType   | `string` | 否   |      | 变量类型(integer/string) |
| varName   | `string` | 否   |      | 变量名                   |
| mergeType | `integer` | 是   | 0    | 合服类型                 |

```lua
-- 引擎启动触发
function startup(sysobj)
    inisysvar("integer","系统变量_1",0)  --声明合区时 保留主区
    inisysvar("integer","系统变量_2",1)  --声明合区时 保留副区
    inisysvar("integer","系统变量_3",2)  --声明合区时 取大
    inisysvar("integer","系统变量_4",3)  --声明合区时 取小
    inisysvar("integer","系统变量_5",4)  --声明合区时 相加
    inisysvar("string","系统变量_6",5)   --声明合区时 相连
    inisysvar("string","系统变量_7",6)   --声明合区时 删除
end
```

