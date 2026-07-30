# 贡献指南

[View English](./CONTRIBUTING.md)

欢迎参与 openJiuwen 社区贡献。openJiuwen 作为开源 Agent 平台，致力于提供灵活、强大且易用的 AI Agent 开发与运行能力。我们鼓励开发者以各种方式参与，包括但不限于代码贡献、文档改进、问题反馈与功能建议。

本指南适用于 [openJiuwen-ai](https://github.com/openJiuwen-ai) 组织下各代码仓的通用协作规范。完整贡献路径还可参考官网：[加入 openJiuwen 开源社区](https://www.openjiuwen.com/contribute)。

## 代码托管说明

GitHub 与 [GitCode 上的 openJiuwen](https://gitcode.com/openJiuwen) 保持双向同步，便于两端开发者浏览与协作。同步范围包括但不限于：

- **代码与文件**：新增、修改、删除等变更会在两端同步。
- **Issue**：在一侧创建、更新、关闭的 Issue，会同步到另一侧。
- **Pull Request / 合并请求**：相关协作信息也会随仓库状态同步。

因此，请避免就同一事项在 GitHub 与 GitCode 两端重复提交 Issue 或 Pull Request，以免产生重复记录或冲突。日常贡献任选一端即可，另一端会自动同步。

## 开始之前

- 参与贡献前，请阅读并遵守 [openJiuwen 社区行为准则](https://github.com/openJiuwen-ai/community/blob/main/openJiuwen社区行为准则.md)。
- 您需要签署 openJiuwen 社区「开发者贡献协议」（CLA），才能参与社区贡献。GitHub 仓库已接入 [CLA Assistant](https://github.com/cla-assistant/cla-assistant)：首次向仓库提交 Pull Request 时，CLA Assistant 会在 PR 下留言并附上签署链接，按提示完成签署即可；签署通过后，后续 PR 一般无需重复签署。
- 在 [openJiuwen-ai](https://github.com/openJiuwen-ai) 中找到您感兴趣的仓库，并先阅读该仓库的 `README` 与相关说明。

## License

[Apache License 2.0 (Apache-2.0)](https://www.apache.org/licenses/LICENSE-2.0)

## 版权规范

用户提交的代码必须是原创内容，不得侵犯他人知识产权，贡献代码请遵守[许可证与版权规范](https://gitcode.com/openjiuwen/community/tree/main/contribute/许可证与版权规范.md)。若新贡献代码涉及第三方开源软件引入或片段引用，请严格遵守[许可证与特殊许可证指引](https://gitcode.com/openjiuwen/community/tree/main/contribute/许可证与特殊许可证评审指导.md)中的要求。

openJiuwen有权根据相关规范修改/删除开发者贡献的内容，直至符合对应规范要求。

## 贡献方式

### 反馈问题

高质量的问题反馈有助于我们不断完善项目质量。您提供的信息越详尽，对我们改进越有帮助。

1. 打开目标仓库的 **Issues** 页面（在 [openJiuwen-ai](https://github.com/openJiuwen-ai) 中进入对应仓库后选择 Issues）。
2. 单击 **New issue**，在标题中简要描述问题，在正文中补充详细说明。
3. 提交后请耐心等待对应维护团队确认与跟进。

> **如何反馈一个高质量的问题？**
>
> - 提供问题的具体位置（模块、文件、文档章节等）与清晰描述，必要时附截图或日志。
> - 说明复现步骤、期望行为与实际行为，以及对用户的影响。
> - 若涉及运行或示例错误，请提供 openJiuwen 相关组件版本、运行环境及完整报错信息。
> - 将问题范围限定在一个具体内容或任务。若牵涉面较大，可拆分为多个小问题。例如：「项目需要优化」过于宽泛，而「XX 模块在 YYY 场景下缺少对 ZZZ 的处理」则足够具体、可操作。
> - 搜索现有问题列表，确认是否已有相关或类似问题。
> - 如果新问题与其他 Issue 或 PR 有关联，可使用完整 URL 或 `#编号` 引用。

### 在线更改

针对少量内容修改和补充（如文案修正、小范围修复），可直接在 GitHub 上在线编辑。

提交步骤：

1. 在 GitHub 上打开目标仓库中的相应文件。
2. 单击文件右上角的铅笔图标（**Edit this file**）。若提示需要 Fork，按指引将仓库 Fork 到个人账号后再编辑。
3. 完成更改，可通过预览确认效果（如适用）。
4. 在页面底部填写简要的变更说明，提交变更并创建 Pull Request。

提交信息建议遵循 [Conventional Commits](https://www.conventionalcommits.org/zh-hans/v1.0.0/)，例如：`fix: handle empty response in runtime`、`docs: fix typo in quickstart`。

对应维护团队将评审并合并您的修改，感谢您对 openJiuwen 的支持。

### 本地更改

适合需要修改或补充较多内容的场景（功能开发、缺陷修复、较大范围文档更新等）。

提交步骤：

1. Fork 目标仓库。
2. Clone 到本地，并基于该仓库的默认分支创建变更分支（常见为 `main` 或 `develop`，以仓库说明为准）。
3. 完成本地修改后，使用带 sign-off 的提交（与已签署 CLA 的邮箱保持一致），例如：

   ```bash
   git commit -sm "feat: add xxx support"
   ```

   示例：`Signed-off-by: user.name <user.email>`

4. 将分支推送到您的 Fork，并在 GitHub 上向原仓库创建 Pull Request。
5. 等待门禁检查与维护团队审核，通过后合入。

**PR 建议说明：** 变更目的与背景、主要改动、测试情况，以及关联的 Issue 编号。

## 社区沟通

如果您在使用或贡献过程中遇到问题，可通过以下渠道联系我们：

- 网站：<https://www.openjiuwen.com>
- 邮箱：contact@openjiuwen.com
- 社区仓库：<https://github.com/openJiuwen-ai/community>
