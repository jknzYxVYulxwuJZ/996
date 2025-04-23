### 调用游戏面板

`openhyperlink`

| 参数    | 类型      | 空   | 默认                | 注释                                                                                                      |
| :------ | :-------- | :--- | :------------------ | :-------------------------------------------------------------------------------------------------------- |
| play    | `object`  | 否   |                     | 玩家对象                                                                                                  |
| nId     | `integer` | 否   |                     | 面板ID                                                                                                    |
| nState  | `integer` | 否   |                     | 0=打开<br />1=打开面板重复点按钮不会关闭,除非主动点关闭按钮(一般做任务配合新手引导用到)<br />2=关闭当前面板ID |
| rankWnd | `integer` | 否   | 引擎64_23.08.30新增 | 面板ID(新排行榜用)                                                                                        |
| isHero  | `integer` | 否   | 引擎64_23.08.30新增 | 0/nil=玩家<br />1=英雄(新排行榜用)                                                                          |

*跳转面板ID参考如下: *
```
        Equip               = 1,            -- 角色-装备
        State               = 2,            -- 角色-状态
        Attri               = 3,            -- 角色-属性
        Skill               = 4,            -- 角色-技能
        Title               = 5,            -- 角色-装备
        BestRing            = 6,            -- 角色-首饰盒
        Bag                 = 7,            -- 背包
        Stall               = 8,            -- 摆摊
        StoreHot            = 9,            -- 商城-热销
        StoreBeauty         = 10,           -- 商城-装饰
        StoreEngine         = 11,           -- 商城-功能
        StoreFestival       = 12,           -- 商城-节日
        GuildMain           = 13,           -- 行会-主界面
        GuildMember         = 14,           -- 行会成员列表
        GuildList           = 15,           -- 行会列表
        Mail                = 16,           -- 邮件
        Team                = 17,           -- 组队
        NearPlayer          = 18,           -- 附近玩家

        Setting             = 23,           -- 设置
        MiniMap             = 24,           -- 小地图
        SkillSetting        = 25,           -- 技能设置
        StoreRecharge       = 26,           -- 充值
        Auction             = 27,           -- 拍卖行
        Friend              = 28,           -- 好友
        ExitToRole          = 29,           -- 小退
        GuildCreate         = 30,           -- 行会创建
        Guild               = 31,           -- 智能行会界面
        Rank                = 32,           -- 排行榜
        Trade               = 33,           -- 面对面交易 请求
        ForceExitToRole     = 34,           -- 强制小退
        TradingBank         = 35,           -- 交易行
        GuideEnter          = 36,           -- 引导进入
        SuperEquip          = 37,           -- 角色-神装
        HeroEquip           = 41,           -- 英雄-装备
        HeroState           = 42,           -- 英雄-状态
        HeroAttri           = 43,           -- 英雄-属性
        HeroSkill           = 44,           -- 英雄-技能
        HeroTitle           = 45,           -- 英雄-称号
        HeroBestRing        = 46,           -- 英雄-首饰盒
        HeroBag             = 47,           -- 英雄-背包
        HeroSuperEquip      = 48,           -- 英雄-神装
        ReinAttrPoint       = 51,           -- 转生属性点
        Chat                = 52,           -- 聊天
        PCPrivate           = 53,           -- PC 私聊记录页

        MagicJointAttack    = 99,           -- 释放合击

        AssistChange        = 110,          -- 主界面-任务栏
        Box996              = 111,          -- 盒子称号
        MainMiniMapChange   = 112,          -- 小地图伸缩
        PCResolution        = 113,          -- PC 分辨率设置
        ChatExtendEmoj      = 114,          -- 角色-表情
        ChatExtendBag       = 115,          -- 聊天小框-背包
        MainNear            = 116,          -- 主界面-附近列表
        CallPay             = 117,          -- 调用-支付

        SettingBasic        = 300,          -- 基础设置
        SettingWindowRange  = 301,          -- 视距
        SettingFight        = 302,          -- 战斗
        SettingProtect      = 303,          -- 保护
        SettingAuto         = 304,          -- 挂机
        SettingHelp         = 305,          -- 帮助

        KeFu                = 310,          -- 调用客服界面
        Compound            = 2201,         -- 合成
```

