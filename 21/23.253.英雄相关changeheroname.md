### 英雄改名接口

`changeheroname`

> **<font color="#808080" style="font-size: 13px;">引擎64_23.10.24新增接口</font>**

| 参数     | 类型     | 空   | 默认 | 注释       |
| :------- | :------- | :--- | :--- | :--------- |
| player   | `object` | 否   |      | 玩家对象   |
| heroName | `string` | 否   |      | 英雄新名字 |
```lua
    changeheroname(player,role_name.."AA英雄")

    --QFunction-0.lua
    function queryingheroname(player)
        sendmsg(player, 1, '{"Msg":"英雄<font color=\'#ff0000\'>正在查询请稍后。。。</font>","Type":9}')
    end
    function queryheronameok(player)
        sendmsg(player, 1, '{"Msg":"英雄<font color=\'#ff0000\'>查询成功，该名称可以使用</font>","Type":9}')
    end
    function changeingheroname(player)
        sendmsg(player, 1, '{"Msg":"英雄<font color=\'#ff0000\'>正在修改请稍后。。。</font>","Type":9}')
    end
    function changeheronameok(player)
        sendmsg(player, 1, '{"Msg":"英雄<font color=\'#ff0000\'>你的名字修改成功</font>","Type":9}')
    end
    function heronameLengthfail(player)
        sendmsg(player, 1, '{"Msg":"英雄<font color=\'#ff0000\'>名字长度不允许超过30个字符！</font>","Type":9}')
    end
    function heronamefilter(player)
        sendmsg(player, 1, '{"Msg":"英雄<font color=\'#ff0000\'>该名字存在非法字符！</font>","Type":9}')
    end
    function heronameexists(player)
        sendmsg(player, 1, '{"Msg":"英雄<font color=\'#ff0000\'>该名字已经被其他玩家占用，请选择其他名字</font>","Type":9}')
    end
    function changeheronamefail(player)
        sendmsg(player, 1, '{"Msg":"英雄<font color=\'#ff0000\'>改名失败！</font>","Type":9}')
    end
```

------------

