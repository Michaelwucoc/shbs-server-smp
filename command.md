---
title: 服务器指令
description: 
published: true
date: 2024-05-06T02:14:13.348Z
tags: 
editor: markdown
dateCreated: 2024-03-20T14:23:28.430Z
---

> **符号说明**
`<  >`表示这个内容您必须填写
`[  ]`表示这个内容您可以选择填写
`*/....`表示这是一个需要升级/有对应权限才可以执行的权限
`^/....`表示这是管理员指令
{.is-info}
# 基本指令
- 登录 `/l <密码>`
- 注册 `/reg <密码> <重复一遍密码>`
> 比如我要使用123456作为密码进行注册: 输入 `/reg 123456 123456`
登录就使用 `/l 123456`
{.is-info}



---
- 传送到玩家 `/tpa <玩家ID>`
- 将玩家传送过来 `/tpahere <玩家ID>`
- 同意传送 `/tpaaccept`
- 拒绝传送 `/tpadeny`
- 自动同意传送 `/tpauto`
- 接受/阻止传送请求 `/tptoggle`
---
- 打开末影箱 `*/enderchest`
- 打开工作台 `*/craft`
- 打开铁砧 `*/anvil`
- 打开死亡菜单 `/grave`
- 自杀 `/suicide`
- 传送到高处 `*/top`
- 维修物品 `*/repair all`
# 礼物
- 给玩家礼物 `/gift <玩家> <物品数量>` 
手上拿着你需要给予的物品

# 动作
- 坐下 `/sit`
- 躺下 `/lay`
- 趴下 `/crawl`

# 设置传送点
- 设置传送点 `/setwarp <传送点名称>`
- 传送到传送点 `/warp <传送点名称>`
- 设置家 `/sethome [名字]`
- 传送到家 `/home [名字]`

# 领地指令
 - 创建领地 `/res create [领地名称]`
 
 TIPS:您可以使用木锄选择区域
 - 自动创建领地 `/res auto [领地名称] [范围]`
 *如果您不填写 范围 ， 那么会自动以您的中心创建您能认领的最大的范围的领地*
 ---
 - 设置传送点 `/res tpset`
 该命令将会把**你所在的位置设置为领地的传送点**,你必须*站在一个领地里*才能使用这个命令,且必须是*领地所有者或者管理员*
 ---
 
 - 设置权限 `/res set <领地名称> [权限] [true/false/remove]`
 	- 显示权限GUI `/res set`
   你必须*站在一个领地里*才能使用这个命令
   
 - 添加信任的玩家 `/res padd <领地名称> [玩家ID]`
 	- 快速添加 `/res padd <玩家ID>`
   你必须 *站在一个领地里* 才能使用这个命令
 - 删除信任的玩家 `/res pdel <领地名称> [玩家ID]`
 	- 快速删除 `/res pdel <玩家ID>`
   你必须 *站在一个领地里* 才能使用这个命令
 ---
 - 传送到领地 `/res tp <领地名称> `
 你必须拥有这个领地的**传送权限**
 
 # 假人 (MVP专属)
>  请不要生成超过2个假人，否则您会失去假人的权限!
假人生成前建议去微信或论坛申请假人ID白名单
{.is-warning}

| 命令            | 作用        | 备注                      |
|---------------|-----------|-------------------------|
| /fp spawn [Name]   | 召唤假人      |                         |
| /fp kill      | 杀死假人      |                         |
| /fp killall   | 杀死服务器所有假人 |                         |
| /fp select    | 选中假人      | 当玩家假人数量 >= 2 时才会出现      |
| /fp selection | 查看选中假人    | 当玩家假人数量 >= 2 时才会出现      |
| /fp list      | 查看已召唤的假人  |                         |
| /fp distance  | 查看与假人的距离  |                         |
| /fp drop      | 丢弃手上一个物品  |                         |
| /fp dropstack | 丢弃手上整组物品  |                         |
| /fp dropinv   | 丢弃背包所有物品  |                         |
| /fp skin      | 复制玩家皮肤    | 非在线玩家有 60 秒冷却           |
| /fp invsee    | 查看假人背包    | 玩家对假人右键同等效果             |
| /fp sleep     | 睡觉        |                         |
| /fp wakeup    | 起床        |                         |
| /fp status    | 查看假人状态    |                         |
| /fp respawn   | 让死亡的假人复活  | 当服务器配置假人死亡时不踢出才会出现      |
| /fp tp        | 传送到假人身边   |                         |
| /fp tphere    | 让假人传送到身边  |                         |
| /fp tps       | 与假人交换位置   |                         |
| /fp set       | 更改假人的配置   |                         |
| /fp config    | 更改默认假人配置  |                         |
| /fp expme     | 吸收假人经验值   |                         |
| /fp attack    | 攻击        |                         |
| /fp mine      | 挖掘        |                         |
| /fp use       | 使用/交互/放置  |                         |
| /fp jump      | 跳跃        |                         |
| /fp turn      | 转身        |                         |
| /fp look      | 看向指定位置    |                         |
| /fp move      | 移动        |                         |
| /fp ride      | 骑乘        |                         |
| /fp sneak     | 潜行        |                         |
| /fp swap      | 交换主副手物品   |                         |
| /fp hold      | 手持对应快捷栏物品 |                         |
| /fp cmd       | 让假人执行命令   | 不给权限的情况下，允许执行配置文件里定义的命令 |

# 照片 (VIP专属)
查看照片信息 `/image describe` 
导入照片 `/image download <链接> <文件名>`
列出可用的照片 `/image list`
放置照片 `/image place <文件名> <大小>`
查看排行榜 `/image top`
## 附:导入图片教程
前往 https://photo.shbsme.top 上传照片
![](https://photo.shbsme.top/i/2024/04/28/662dfad80d3bc.png)
复制URL，在游戏内使用导入照片指令，URL填写复制的链接。 文件名不要重复！



 

