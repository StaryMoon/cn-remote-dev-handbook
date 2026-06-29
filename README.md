# 中文远程开发与服务器手册

![preview](assets/preview.png)

学生服务器、实验室 GPU、远程机器，出问题通常不是大问题，就是 SSH 连不上、端口转不出来、文件传一半断了。这个仓库按排障和日常使用来收工具。

长任务不上 tmux，迟早会吃一次亏。端口裸奔公网，也迟早会吃一次亏。

## 先看这几个

VS Code Remote SSH / Tailscale / Cloudflare Tunnel / ngrok

先把 SSH key、tmux、rsync 三件事弄稳，再考虑花哨的隧道和组网。

## 入口

| 名称 | 我为什么留它 |
| --- | --- |
| [VS Code Remote SSH](https://code.visualstudio.com/docs/remote/ssh) | VS Code 远程开发官方文档。 |
| [Tailscale](https://tailscale.com/) | 基于 WireGuard 的组网工具。 |
| [Cloudflare Tunnel](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/) | 无需公网 IP 的隧道方案。 |
| [ngrok](https://ngrok.com/) | 本地服务公网暴露工具。 |
| [tmux](https://github.com/tmux/tmux) | 终端会话复用。 |
| [mosh](https://mosh.org/) | 弱网下更稳的远程 shell。 |
| [rsync](https://rsync.samba.org/) | 增量文件同步。 |
| [rclone](https://rclone.org/) | 云盘和远程存储同步工具。 |

## 我的使用顺序

- 先保证 SSH key 登录稳定。
- 长任务必须用 tmux。
- 跨网络访问优先考虑 Tailscale 或 Cloudflare Tunnel。

## 别踩坑

- 不要把端口裸奔到公网。
- 不要把私钥上传到服务器或网盘。

## 截图来源

这张图来自公开页面：[https://tailscale.com/](https://tailscale.com/)。如果页面改版，截图可能会和当前官网略有出入。

## 维护方式

链接数据放在 [`data/links.json`](data/links.json)。我倾向于少而准：入口失效就换，说明过时就改，不把这里做成什么都往里塞的大杂烩。

## License

MIT. 第三方商标、页面截图和网站内容归原权利方所有；本仓库只做中文导航和使用笔记。
