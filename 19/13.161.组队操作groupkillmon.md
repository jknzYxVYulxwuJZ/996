### 组队杀死怪物时触发

`groupkillmon`

| 参数    | 类型     | 空   | 默认                | 注释     |
| :------ | :------- | :--- | :------------------ | :------- |
| actor   | `object` | 否   |                     | 玩家对象 |
| monName | `string` | 否   | 引擎64_24.08.07新增 | 怪物名字 |
```lua
--组队杀死怪物(同地图内成员每人触发一次)
function groupkillmon(actor,monName)
    say("组队杀死怪物时触发", getbaseinfo(actor, 1),monName)
end
```

------------

## 接口

