# 职场对话透镜

> 看懂职场消息里的诉求，预演关键对话，把项目往前推。

「明早确认负责人」是在通知你，还是需要你现在行动？要报延期、提方案或争取资源，怎么开口更清楚？职场对话透镜是一款 WorkBuddy 专家，可以先解读消息，再模拟对话，最后给出可调整的回复草案。

[RC8 试装包](https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases/tag/v0.5.0-rc8) · [历史版本](https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases)

## 可以做什么

| 场景 | 用法 |
| --- | --- |
| 解码消息 | 区分字面、推测和待确认项，给出回复草案，保留你已经确认的责任和条件。 |
| 陪练对话 | 模拟对方追问，适合练习汇报进度、报风险或协调资源。回复标明画像和模拟状态。 |
| 训练画像 | 提交去标识化的协作特征，审阅后发布。使用中的会话固定画像和版本。 |
| 分享协作建议 | 预览并确认受众后导出审阅过的建议。分享稿可独立阅读，原始材料和证据锚点由提供者保管。 |

## 安装

1. 用有仓库访问权限的 GitHub 账号下载 [RC8 安装 ZIP](https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases/download/v0.5.0-rc8/workplace-dialogue-lab-v0.5.0-rc8.zip) 和 [SHA-256 校验文件](https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases/download/v0.5.0-rc8/workplace-dialogue-lab-v0.5.0-rc8.zip.sha256)。
2. 核对 SHA-256 后解压。Windows 双击 `install-windows.cmd`，macOS 打开 `install-macos.command`。需要 WorkBuddy 和 Python 3.9 或更新版本。
3. 在 WorkBuddy 专家中心打开「职场对话解读与陪练」，选合成示例或通用模式即可体验。

## 试一句

> 日常使用合成示例。解码：对方说「会上再定谁来接」。我该怎么回？

草案示例「收到，结果出来后请同步一下。」

也可以说「陪练：我需要向上汇报延期，请扮演对方追问」。如果想让专家用完整规则重新处理上一轮，输入「用完整提示重跑」。

## 试装状态

RC8 已通过本地回归，并在 macOS WorkBuddy 用 DeepSeek V4.1 Flash 完成五道合成解码题的双模式检查。Windows 实机待测。曾出现一次完整重跑显示完成但正文空白，重试及之后三次独立复查均返回正文。详见[预发行说明](https://github.com/henry-tinker-ai/workplace-dialogue-lab/releases/tag/v0.5.0-rc8)。

工具面向向上管理、项目推进和职场协作。材料请先去标识化，模拟内容仅用于练习。试装适用安装包内许可。

首页组织方式参考[老板 Skill](https://github.com/vogtsw/boss-skills)。
