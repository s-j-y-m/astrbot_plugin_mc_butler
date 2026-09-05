<p align="center">
  <img src="LOGO.png" width="180" alt="MC 服务器大管家">
</p>

# astrbot_plugin_mc_butler（MC 服务器大管家）

> QQ 群里的 MC 服务器大管家：QQ绑定MC账号、远程执行服务器指令、查看子服状态，@机器人 说人话就能用。

## ✨ 功能

- 🔗 **QQ ↔ MC 账号绑定** —— 绑定即进服白名单，未绑定玩家由 Velocity 代理自动拦截
- ⌨️ **远程执行指令** —— 管理员在 QQ 里直接发服务器指令（如 `!!pb list`），输出原样回显
- 📡 **子服状态查询** —— 在线人数、玩家名单、MOTD 一眼看清
- 💬 **自然语言操作** —— LLM 工具调用，“回档到 3 号存档”这类话直接听懂（危险操作需 QQ 侧二次确认）
- 🖥️ **独立 WebUI** —— 浏览器里管理绑定与动作对照表

## 📦 安装

1. AstrBot ≥ v4.10.4：插件市场搜索「MC 服务器大管家」，或从本仓库安装
2. 配套组件在 [Releases](https://github.com/s-j-y-m/astrbot_plugin_mc_butler/releases) 下载：
   - Velocity 代理装 `mclink-velocity`（进服拦截 + HTTP/RCON 指令桥）
   - 每个子服的 MCDR 装 `rcon_bridge`（RCON 服务端）

## 🚀 快速上手

| 指令 | 说明 |
|---|---|
| `/bind <MC ID>` | 绑定你的 MC 账号 |
| `/mcm ping [服务器]` | 查看子服状态 |
| `/mcm c [服务器] <指令>` | 管理员远程执行指令 |
| `/mcm help` | 完整指令帮助 |

在插件配置中填好 Velocity 地址与 token 即可使用。

## 📖 完整说明

配置项详解、整体架构、自然语言前置条件、回档二次确认流程、动作对照表、独立 WebUI 等，见 **[完整说明](完整说明.md)**。
