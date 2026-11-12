# 职场对话透镜

> 看懂职场消息里的诉求，预演关键对话，把项目往前推。

「明早确认负责人」是在通知你，还是需要你现在行动？要报延期、提方案或争取资源，怎么开口更清楚？职场对话透镜是一款 WorkBuddy 专家，可以先解读消息，再模拟对话，最后给出可调整的回复草案。

[RC9 试装包](https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases/tag/v0.5.0-rc9) · [历史版本](https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases)

## 可以做什么

| 场景 | 用法 |
| --- | --- |
| 解码消息 | 区分字面、推测和待确认项，给出回复草案，保留你已经确认的责任和条件。 |
| 陪练对话 | 模拟对方追问，适合练习汇报进度、报风险或协调资源。回复标明画像和模拟状态。 |
| 训练画像 | 提交去标识化的协作特征，审阅后发布。使用中的会话固定画像和版本。 |
| 分享协作建议 | 预览并确认受众后导出审阅过的建议。分享稿可独立阅读，原始材料和证据锚点由提供者保管。 |

## 安装

1. 从上方 RC9 发行页下载 ZIP 和 SHA-256 校验文件，核对后解压。PowerShell 用 `Get-FileHash -Algorithm SHA256 <zip>` 并比对校验值；Git Bash 用 `sha256sum -c <zip>.sha256`；macOS 用 `shasum -a 256 -c <zip>.sha256`。
2. 需要 WorkBuddy 和 Python 3.9 或更新版本。Windows 在包目录运行 `python scripts\install_release.py`，也可双击 `install-windows.cmd`（双击入口尚待实机确认）。批处理查找 Python、运行同一个安装器并暂停显示结果。macOS 打开 `install-macos.command`。
3. 在「我的专家」找「职场对话透镜」（职业标注「职场对话解读与陪练」），选择「合成示例」或「通用」。

### Windows 排错

- 附件下载遇到 TLS 握手失败时，使用浏览器打开发行页下载并校验。
- RC9 会自动检查各固定磁盘上的 WorkBuddy 常见安装路径。若仍提示缺少官方组件，可用 `--official-scripts` 指定官方脚本目录，详见包内 `INSTALL-GITHUB.md`。
- 若策略拦截批处理，可直接运行上面的 Python 入口。

## 试一句

> 日常使用合成示例。解码：对方说「会上再定谁来接」。我该怎么回？

草案示例「收到，结果出来后请同步一下。」

也可以说「陪练：我需要向上汇报延期，请扮演对方追问」。如果想让专家用完整规则重新处理上一轮，输入「用完整提示重跑」。

## 试装状态

RC8 已通过本地回归，并在 macOS WorkBuddy 用 DeepSeek V4.1 Flash 完成五道合成解码题的双模式检查。RC9 在 Windows 隔离配置中已通过 SHA-256 校验、自动定位 E 盘 WorkBuddy 官方组件、官方校验及 marketplace.json 注册。批处理双击、专家界面人工打开及一句话代装仍待确认。曾出现一次完整重跑显示完成但正文空白，重试及之后三次独立复查均返回正文。详见[预发行说明](https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases/tag/v0.5.0-rc8)。

工具面向向上管理、项目推进和职场协作。材料请先去标识化，模拟内容仅用于练习。RC9 适用安装包内的个人非商用许可和 GitHub 公开分发补充许可。

首页组织方式参考[老板 Skill](https://github.com/vogtsw/boss-skills)。


## 用一句话安装

在普通 WorkBuddy 新会话粘贴：

> 帮我安装 WorkBuddy 专家「职场对话透镜」：https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases/tag/v0.5.0-rc9

请 WorkBuddy 下载并核对同版本 ZIP 和 SHA-256，解压后按上述步骤安装。如果附件下载失败，可用浏览器下载再交给 WorkBuddy。安装后在「我的专家」找「职场对话透镜」。


## WorkBuddy 模型建议

做即时文字陪练时，推荐优先使用 **Hy4**。在一次同题盲测中，Hy4 的回复更贴近真实聊天口吻，整轮等待时间也更长。
