### 给视野内玩家发送自定义广播消息

`setotherparams`

| 参数     | 类型      | 空   | 默认 | 注释        |
| :------- | :-------- | :--- | :--- | :---------- |
| play     | `object`  | 否   |      | 玩家对象    |
| varIdx   | `integer` | 否   |      | 属性id(1~5) |
| varValue | `integer` | 否   |      | 属性值      |
```lua
    [[服务端]]
    setotherparams(actor,1,3)
    -- setotherparams(actor,2,256)
    setotherparams(actor,2,414)

    [[客户端]]
    SL:RegisterLUAEvent(LUA_EVENT_ACTOR_GMDATA_UPDATE, "ACTOR_GM_DATA", function (tab)
        SL:dump(tab,"自定义数据改变")
        SL:dump(SL:GetMetaValue("ACTOR_GM_DATA",tab.id),"获取actor的GM自定义数据")
    end)
    [[足迹示例]]
    local function moveEvent(data)
        local actorID = data and data.id
        if actorID then
            local posX = SL:GetMetaValue("ACTOR_POSITION_X", actorID)
            local posY = SL:GetMetaValue("ACTOR_POSITION_Y", actorID)
            local dir = SL:GetMetaValue("ACTOR_DIR", actorID)
            local effectModel = SL:GetMetaValue("ACTOR_GM_DATA", actorID)[1]
            local effectID = SL:GetMetaValue("ACTOR_GM_DATA", actorID)[2]
            if effectID ~= 0 and posX and posY then
                local actBegin = data.act
                if actBegin == 1 or actBegin == 6 or actBegin == 17 then
                    local eff = GUI:Effect_Create(GUI:Attach_SceneB(), string.format("foot_effect%s_%s%s", actorID, posX, posY), posX, posY, effectModel, effectID, 0,0 , dir, 0.8)
                    GUI:setScale(eff, 0.3)
                    if eff then
                        GUI:Effect_addOnCompleteEvent(eff, function()
                            GUI:removeFromParent(eff)
                        end)
                    end
                end
            end
        end
    end
    SL:RegisterLUAEvent(LUA_EVENT_PLAYER_ACTION_BEGIN, "GUIUtil", moveEvent)
    SL:RegisterLUAEvent(LUA_EVENT_NET_PLAYER_ACTION_BEGIN, "GUIUtil", moveEvent)
```

------------

