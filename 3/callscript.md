### 调用TXT脚本命令
`callscript`

&lt;font color="#ff00ff" style="font-family: Fixedsys;font-size: 15px;"&gt;**特殊：该接口为异步调用,且消耗大,推荐使用callscriptex**&lt;/font&gt;

| 参数     | 类型      | 空   | 默认 | 注释     |
| :------- | :-------- | :--- | :--- | :------- |
| player   | `object`  | 否   |      | 玩家对象 |
| filename | `string`  | 否   |      | 文件名   |
| label    | `integer` | 否   |      | 标签     |
```lua
    [[表示调用执行“测试.txt”文件中的[@测试]标签内容
    “测试.txt”默认读取 Mir200\Envir\Market_def\ 文件夹下，如果有子文件夹，则加载文件名之前]]
    callscript(actor, '测试'， '@测试') 

    [["测试.txt" 位于 Mir200\Envir\Market_def\盟重\ 文件夹下]]
    callscript(actor, '盟重/测试'， '@测试') 
```

