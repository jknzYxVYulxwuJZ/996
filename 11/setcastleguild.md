### 脚本命令设置沙巴克归属

`setcastleguild`

| 参数  | 类型     | 空   | 默认 | 注释                                              |
| :---- | :------- | :--- | ---- | ------------------------------------------------- |
| guildName  | `string` | 否   |      | 行会名称                                          |
| param | `int`    | 否   |      | 是否忽略触发@beforgetcastle<br />0=不忽略<br />1=忽略 |
```lua
setcastleguild("对对对", 0)

--QFunction-0.lua
function beforgetcastle(sysObj,guildName)
    release_print("行会名",guildName)
end
```

------------

