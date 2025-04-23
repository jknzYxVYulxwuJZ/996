### 检测当前人物是否在跨服的地图

`checkkuafu`

| 参数  | 类型  | 空   | 默认 | 注释     |
| :---- | :---- | :--- | :--- | :------- |
| actor | `obj` | 是   |      | 玩家对象 |
```lua
        local isKuafuMap = checkkuafu(actor)
        release_print("当前人物是否在跨服的地图",type(isKuafuMap),tostring(isKuafuMap))
```

<br />

