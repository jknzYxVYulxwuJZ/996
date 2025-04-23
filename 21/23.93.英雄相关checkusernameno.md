### 英雄取名失败触发
`checkusernameno`

|参数|类型|空|默认|注释|
|:----    |:-------    |:--- |----|------      |
|play     |`object`      |否   |    |玩家对象 |

```lua
    local role_name = getbaseinfo(actor,1)
    local hero_name = role_name.."A英雄"
    checkheroname(actor,hero_name)

    [[英雄取名成功触发]]
    function checkusernameok(actor)
        release_print("英雄取名成功触发,之后去创建英雄")
        local job,sex = getbaseinfo(actor,7),getbaseinfo(actor,8)
        local role_name = getbaseinfo(actor,1)
        local hero_name = role_name.."A英雄"
        createhero(actor, hero_name, job, sex)
    end
    
    [[英雄取名失败触发]]
    function checkusernameno(actor)
        sendmsg(actor, 1, '{"Msg":"<font color=\'#ff0000\'>英雄名字已经存在</font>","Type":9}')
    end

    [[英雄创建触发]]
    function createherook(actor)
        release_print("创建成功,召唤英雄")
        recallhero(actor)
    end

    [[英雄登陆触发]]
    function herologin(actor)
        release_print("英雄登陆")
    end
```

## 接口

