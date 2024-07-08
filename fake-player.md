---
title: 假人
description: 
published: true
date: 2024-07-08T14:07:58.226Z
tags: 
editor: markdown
dateCreated: 2024-04-24T14:21:00.887Z
---

# 说明
假人是为了给予有能力的玩家更高级的生电体验。仅**MVP**能够使用本功能。
要查看相关指令，请前往 [服务器指令](/command)。

# 创建假人
## 在你创建假人之前
1. 你需要获得赞助并且确认在赞助有效期内
> 填写提示：目前支持 fake2 - fake 20 的创建，需要自定义请联系腐竹。
{.is-info}
## 进入游戏生成假人
1. 进入游戏服务器，站在需要生成假人的方块上
2. 输入命令 `/fp spawn <假人名字>`. 例如: `/fp spawn Example`
![](http://photo.shbsme.top/i/2024/04/24/6629134be6dd3.png)

## 传送假人到你的位置
1. 由于登陆插件性质，您需要使用 `/fp tphere <假人名字>` 例如： `/fp tphere Example`
![](http://photo.shbsme.top/i/2024/04/24/662913b7011ae.png)

即可创建一个假人
![](http://photo.shbsme.top/i/2024/04/24/662913e769fde.png)

# 其他操作
## 看向实体
要获得像自动打怪的效果，您需要设置自动看向附近实体。您可以输入 `/fp look entity once <假人名字>`来让假人看向附近的实体（一次）。如果您需要持续让假人看向附近的实体，请输入`/fp look entity continuous <假人名字>`即可。
## 自动攻击
要实现自动攻击，您可以输入`/fp attack continuous <假人名字>`来实现持续的攻击，直到输入`/fp attack stop <假人名字>`
## 打开物品栏
正常情况下，右键假人即可打开物品栏。
## 打开状态
输入 `/fp status <假人名字>` 即可查看状态：
![](http://photo.shbsme.top/i/2024/04/24/662915272f2a2.png)
您可以点击`<--拿来吧你`来获得假人经验。