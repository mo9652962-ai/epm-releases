# 📦 AI 英语刷题机 — 更新分发仓库

> **本仓库仅存放 Release 安装包与更新元数据，不含源码。**

## 这是什么

[AI 英语刷题机](https://github.com/mo9652962-ai/english-multiple-choice-practice-machine) 的自动更新源。
应用通过 `electron-updater` 检查本仓库 Releases，实现 **Windows 一键自动更新**。

## 版本策略

| 渠道 | 命名 | 说明 |
|:---|:---|:---|
| 正式版 | `v1.x.x` | 稳定发布 |
| 内测版 | `v2.0.0-beta.x` | 新功能内测 |

## 双源更新（国内加速）

应用自动切换更新源，解决国内网络访问 GitHub 慢/不通的问题：

1. **主源**：GitHub Releases（本仓库）
2. **镜像源**：`ghproxy.net` 代理（国内直连）

检测到主源失败时自动切换到镜像源，无需手动配置。

## 文件说明

```
epm-setup-<版本>.exe         Windows 安装包（nsis，含自动更新）
epm-portable-<版本>.exe      便携版（免安装）
latest.yml                    electron-updater 元数据（勿手动修改）
```

## 安全

- 所有安装包均使用 **Authenticode 代码签名**（SHA256）
- 首次安装如遇 SmartScreen 提示，选择"更多信息 → 仍要运行"
- 若企业环境签名校验失败，运行安装目录下 `一键信任设置.bat`

---

*本仓库由 Hermes Agent 自动维护 — 每次发布自动生成 Release + 更新元数据。*
