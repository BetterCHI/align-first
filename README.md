# align-first · 先对齐，再动手

**别等 AI 做完一大轮，才发现方向不对。先问清，再开工。**

一个轻量需求对齐 Skill：优先每轮问 1 个关键问题，明确你要什么、是否可行、怎样才算满意，最后交付一份执行简报。

[⬇ 一键下载](https://github.com/BetterCHI/align-first/archive/refs/tags/v1.0.0.zip) · [复制安装提示词](INSTALL_PROMPT.md) · [查看技能](align-first/SKILL.md) · [⭐ 支持项目](https://github.com/BetterCHI/align-first)

## 复制给你的 Agent，安装后直接开始

```text
请安装并启用需求对齐技能：https://github.com/BetterCHI/align-first/tree/v1.0.0/align-first 。先读取其中的 SKILL.md，优先使用 skill-installer，按当前 Agent 的用户级技能规范安装。仅添加本技能；同名同内容则复用，有差异先保留并询问。完成后核对文件、报告实际安装位置，并读取技能在本对话开始使用：先问我想完成什么，每轮优先1个关键问题，只澄清需求，收到明确开工指令再制作。纯聊天环境则读取该仓库的 COPY_PROMPT.md，按其流程提问并标注“会话使用”。
```

仓库地址：[BetterCHI/align-first](https://github.com/BetterCHI/align-first)。安装提示词固定到 `v1.0.0`，便于复现；原生技能发现机制依当前 Agent 而定，安装后读取技能即可在当前对话按流程使用。

## 它怎么工作

你的模糊想法 → 关键问题 → 目标与验收标准 → 执行简报 → 你明确要求后再开工。

- 已经讲过的内容，跳过重复提问。
- 把“高级、好看、专业”转成参考特征或可检查标准。
- 分清已验证、待验证和阻塞项，而不是盲目承诺。
- 普通“可以 / 对”只确认需求，不自动启动正式制作。

核心技能为单文件；没有依赖包、联网服务或账户配置。实际速度、token 消耗和效果取决于使用的模型与任务，本项目重点是减少需求错配与返工。

## 下载与使用

### Codex 用户

1. 在仓库页面点击 **Code → Download ZIP**，然后解压。
2. 把其中含有 `SKILL.md` 的 **align-first 文件夹**交给 Codex，发送：

   ```text
   请将我提供的 align-first 文件夹安装为当前用户的全局 skill，保留原有同名技能并提示我处理冲突。
   ```

3. 安装成功后，在下一轮对话输入：

   ```text
   $align-first 我想做一个产品介绍页，先帮我问清楚。
   ```

也可以直接把本仓库链接发给 Codex：

```text
请使用 skill-installer，安装上面 GitHub 仓库中的 align-first 子目录。
```

分享 ZIP 中的技能文件夹同样适用。只需安装技能文件夹，其余文件是给人看的说明。

### 普通聊天 AI 用户

打开 [COPY_PROMPT.md](COPY_PROMPT.md)，复制全文发给 AI，再说自己的需求。也可以上传该文件并要求按其中的需求澄清流程提问；这是聊天提示词用法，不代表安装了原生 Skill。

## 支持这个项目

如果它帮你减少了返工，欢迎登录 GitHub，点击本仓库右上角 **☆ Star**，方便收藏，也支持后续更新。

下载与 Star 是独立操作，下载即用，星标自愿。

## 官方说明

- [GitHub ZIP 下载](https://docs.github.com/en/repositories/working-with-files/using-files/downloading-source-code-archives)
- [GitHub Star](https://docs.github.com/en/get-started/exploring-projects-on-github/saving-repositories-with-stars)
