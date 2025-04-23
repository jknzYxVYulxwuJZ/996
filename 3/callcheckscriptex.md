### 调用传奇脚本命令
`callscriptex`

| 参数       | 类型     | 空   | 默认 | 注释         |
| :--------- | :------- | :--- | :--- | :----------- |
| player     | `object` | 否   |      | 玩家对象     |
| scriptname | `string` | 否   |      | 脚本接口     |
| arr        | `any`    | 否   |      | 参数1~参数10 |

```lua
function main(self)
  callscriptex(self, "SENDMSG", 0, "缝合怪")
end
```

`callcheckscriptex`

| 参数       | 类型     | 空   | 默认 | 注释           |
| :--------- | :------- | :--- | :--- | :------------- |
| player     | `object` | 否   |      | 玩家对象       |
| scriptname | `string` | 否   |      | 脚本接口       |
| arr        | `any`    | 否   |      | 参数1~参数10   |
| result     | `bool`   | 是   |      | 返回值，布尔值 |

------------

