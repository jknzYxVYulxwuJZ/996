### 获取玩家好友列表
`getfriendnamelist`

| 参数   | 类型     | 空   | 默认 | 注释           |
| :----- | :------- | :--- | :--- | :------------- |
| play   | `object` | 否   |      | 玩家对象       |
| result | `table`  | 否   |      | 好友的名字列表 |
```lua
    local list = getfriendnamelist(actor)
    for key, value in pairs(list or {}) do
        release_print(key,value)
    end
```

---

