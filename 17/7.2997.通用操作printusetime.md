### 打印脚本总耗时(微秒)

- 需要角色游戏权限为10,且需退出管理员模式(GM命令)

`printusetime`

| 参数   | 类型      | 空   | 默认 | 注释                                     |
| :----- | :-------- | :--- | :--- | :--------------------------------------- |
| play   | `object`  | 否   |      | 玩家对象                                 |
| on/off | `integer` | 否   |      | 1=开始计时<br />2=结束计时，并打印耗时信息 |

```lua
printusetime(actor,1)
for i = 1, 100, 1 do
    release_print("打印耗时",i)
end
printusetime(actor,2)
```

