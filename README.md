# 中文远程开发与服务器手册

> SSH、远程编辑、文件同步、隧道、tmux 和跨设备组网工具整理。

![preview](assets/preview.png)

## Overview

整理 SSH、远程编辑、文件同步、隧道、终端复用和跨设备组网工具。

本仓库只保留与主题直接相关、入口稳定、说明清晰的资源。优先收录官方文档、主流开源仓库、长期可访问的产品页面和常用工具链。

## Key Resources

VS Code Remote SSH / Tailscale / Cloudflare Tunnel / ngrok

## Resources

| Resource | Use case |
| --- | --- |
| [VS Code Remote SSH](https://code.visualstudio.com/docs/remote/ssh) | VS Code 远程开发官方文档。 |
| [Tailscale](https://tailscale.com/) | 基于 WireGuard 的组网工具。 |
| [Cloudflare Tunnel](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/) | 无需公网 IP 的隧道方案。 |
| [ngrok](https://ngrok.com/) | 本地服务公网暴露工具。 |
| [tmux](https://github.com/tmux/tmux) | 终端会话复用。 |
| [mosh](https://mosh.org/) | 弱网下更稳的远程 shell。 |
| [rsync](https://rsync.samba.org/) | 增量文件同步。 |
| [rclone](https://rclone.org/) | 云盘和远程存储同步工具。 |

## Recommended Path

1. 先保证 SSH key 登录稳定。
2. 长任务必须用 tmux。
3. 跨网络访问优先考虑 Tailscale 或 Cloudflare Tunnel。

## Notes

- 避免将服务端口直接暴露到公网。
- 私钥不得上传到服务器、网盘或公共仓库。

## Screenshot

Source: [https://tailscale.com/](https://tailscale.com/)

## Data

Structured resource data is available in [`data/links.json`](data/links.json).

## Contributing

PRs are welcome for official links, documentation updates, screenshot refreshes, and concise use-case descriptions. Please avoid mirrors, cracked software, referral links, and unverified downloads.

## License

MIT. Third-party trademarks, screenshots, and website content belong to their respective owners.
