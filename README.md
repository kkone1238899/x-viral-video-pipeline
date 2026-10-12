# 流水线 / 生产管线

> 一条视频做一下午？这个库收集一句话到成片的自动化生产管线，每条都写清楚能帮你解决什么、怎么用它搞钱。
>
> A curated collection of production pipelines prompts & skills for viral short videos, gathered from practitioners sharing on X.
> 
> Each entry answers two questions: what problem it solves (and who it's for), and how to make money with it.
> 
> Star counts verified via GitHub API on 2026-10-12. Continuously updated.

## 条目

### Huobao Drama（chatfire-AI/huobao-drama）

**核心提炼**
- 解决什么问题：一句话或一部小说进去，剧本→角色设计→分镜拆分→成片合成，整条短剧流水线在一个平台里走完；四个内置 Agent 分别负责小说改剧本、抽取角色/场景/道具、分镜拆分、生成生图/生视频提示词。
- 核心用法（4 步）：1) 下载桌面版（macOS / Windows）或 Docker 部署；2) 在「设置」里填入模型 API Key（一键写三个常用配置）；3) 新建项目，输入一句话或小说，Agent 自动完成角色设计和分镜拆分；4) 逐集检查确认后，合成整集导出成片。
- 什么时候用 / 常见坑：适合想从 0 搭短剧生产工作室、批量出剧的人；协议为 CC BY-NC-SA 4.0（非商业），拿它接单前先看清授权；需要自备文本 / 图像 / 视频三类模型 API。

**适用场景**：短剧团队、内容工作室、想批量产出短剧的创业者。

**怎么用它搞钱**：短剧批量生产 / 小说推文。

**来源**：[chatfire-AI/huobao-drama](https://github.com/chatfire-AI/huobao-drama) · ⭐16087 · 更新于 2026-10-05

### AutoClip（zhouxiaoka/autoclip）

**核心提炼**
- 解决什么问题：把播客、访谈、课程等长视频自动剪成短视频，一并生成字幕、封面和发布文案，适配抖音、小红书、TikTok、Reels、YouTube Shorts。
- 核心用法（4 步）：1) 下载桌面版（安装包自带 Python 和 FFmpeg，免配环境）；2) 在设置里选模型服务商、填 API Key 并测试连接；3) 贴一个长视频链接，选好平台版式；4) 预览自动成片，检查字幕和取景后下载发布包或直发。
- 什么时候用 / 常见坑：做课程切片、知识博主矩阵号时用；软件免费、云端模型按量计费，量产前先算清费用；Intel Mac / Linux 建议走 Docker 或 CLI 版。

**适用场景**：知识付费从业者、课程切片代运营、要做多平台分发的人。

**怎么用它搞钱**：知识付费 / 课程切片代运营。

**来源**：[zhouxiaoka/autoclip](https://github.com/zhouxiaoka/autoclip) · ⭐9345 · 更新于 2026-10-12

### Jellyfish（Forget-C/Jellyfish）

**核心提炼**
- 解决什么问题：AI 短剧的端到端生产工作台——脚本理解、分镜拆分、角色/场景/道具/服装一致性管理、镜头级生图生视频、异步任务跟踪都在一个界面里，专治"换镜头人物就变脸"。
- 核心用法（4 步）：1) 用 Docker Compose 起前后端服务；2) 导入剧本，AI 拆镜头并抽出角色、场景、道具、服装；3) 为每个镜头准备候选素材（人物图、关键帧），确认状态变为 ready；4) 生成镜头级视频并导出。
- 什么时候用 / 常见坑：短剧已经有一定产量、一致性问题开始拖慢交付时用；它本质是偏生产管理的自建工具，需要自己准备服务器和模型。

**适用场景**：短剧工作室、想把短剧流程工具化的制作团队。

**怎么用它搞钱**：短剧工作室降本接单。

**来源**：[Forget-C/Jellyfish](https://github.com/Forget-C/Jellyfish) · ⭐6701 · 更新于 2026-07-30

### Automate Faceless Content（cporter202/automate-faceless-content）

**核心提炼**
- 解决什么问题：一份"无真人出镜内容自动化"的完整课程指南（10 个模块，4–6 周课表），从入门、工具配置、选题脚本做到变现和规模化，按步带新手做出第一条无出镜视频。
- 核心用法（4 步）：1) 读 Getting Started 指南，了解无出镜内容的逻辑；2) 按 Account Setup 注册并配置生成工具；3) 跟着 Your First Video 做出第一条视频；4) 按 Monetization 章节逐个平台开通收益（YouTube 收益、联盟营销等）。
- 什么时候用 / 常见坑：适合零基础、想按课表学完的人；它深度绑定自家商业工具 ViralWave Studio（有免费试用），工具推荐偏向它家——介意绑定的话，只取课程框架和方法论。

**适用场景**：零基础想做 YouTube / TikTok 无出镜账号的人。

**怎么用它搞钱**：养生 / 故事号矩阵。

**来源**：[cporter202/automate-faceless-content](https://github.com/cporter202/automate-faceless-content) · ⭐3128 · 更新于 2026-06-04

### AI Faceless Video Generator（SamurAIGPT/AI-Faceless-Video-Generator）

**核心提炼**
- 解决什么问题：输入一个话题，自动生成脚本、配音，再用 SadTalker 让一张人脸图"说话"，一条流程跑完就是一条口播视频，全程不用真人出镜。
- 核心用法（4 步）：1) 在 Colab 里打开官方笔记本（官方推荐，省去本地配 GPU）；2) 填入 OpenAI API Key；3) 输入话题和一张人脸图（可用任意头像）；4) 跑完全部 cell，下载成片。
- 什么时候用 / 常见坑：想快速验证口播选题时用；需要 OpenAI API Key，SadTalker 对 GPU 有要求（走 Colab 可绕过）；配音走 gTTS，中文号先跑一条试听再决定。

**适用场景**：想快速测试口播选题的个人创作者、口播号代做。

**怎么用它搞钱**：口播号代做。

**来源**：[SamurAIGPT/AI-Faceless-Video-Generator](https://github.com/SamurAIGPT/AI-Faceless-Video-Generator) · ⭐514 · 更新于 2026-09-17

### Lingjian Video / 灵剪（dososo/blcaptain-lingjian-video）

**核心提炼**
- 解决什么问题：一句话生成发布级中文短视频（脚本、配音、画面、配乐、字幕、音效全自动），但和黑箱出片相反——脚本、配音、画面三关都停下来给你审，逐关确认才继续。
- 核心用法（4 步）：1) 本地运行，配好 LLM、语音和画面模型 Key（`doctor` 会告诉你缺什么、怎么补）；2) 一句话说清目标（平台、主题、比例、内容依据）；3) 逐关确认：脚本关挑版本 → 配音关试听选音色 → 画面关看分镜确认单，每关点头才进下一关；4) FFmpeg 渲染，QA 全绿后导出多平台分发包。
- 什么时候用 / 常见坑：接客户商单、对成片质量有要求、怕黑箱返工时用；它是 CLI / agent 驱动的工程工具，需要一定技术动手力；审批用签名绑定产物内容，内容一改批准自动失效（防偷工减料，也是改一句就要重审整关的代价）。

**适用场景**：接商单的视频创作者、本地商家探店代运营、有技术动手力的个人。

**怎么用它搞钱**：本地商家探店代运营。

**来源**：[dososo/blcaptain-lingjian-video](https://github.com/dososo/blcaptain-lingjian-video) · ⭐255 · 更新于 2026-07-20

## 收录标准

- 来源：X 博主实战分享（原帖 / 评论区 / 引用链）及 GitHub 高星项目
- 每条格式：核心提炼（解决什么问题 / 核心用法 3–5 步 / 什么时候用与常见坑）+ 适用场景 + 「怎么用它搞钱」+ 来源（Star 数与最近更新时间）
- Star 数与更新时间为 2026-10-12 经 GitHub API 核验；持续收录中
- 去重：同一项目只收录一次，不堆 raw 链接

## 相关分类

- 总索引：[x-viral-video-skills](https://github.com/kkone1238899/x-viral-video-skills) —— 13 个分类导航
- [x-viral-video-scripts](https://github.com/kkone1238899/x-viral-video-scripts) —— 编剧 / 脚本
- [x-viral-video-hooks](https://github.com/kkone1238899/x-viral-video-hooks) —— 标题 / 5 秒钩子
- [x-viral-video-creative-direction](https://github.com/kkone1238899/x-viral-video-creative-direction) —— 创意总监
- [x-viral-video-directing](https://github.com/kkone1238899/x-viral-video-directing) —— 导演
- [x-viral-video-replication](https://github.com/kkone1238899/x-viral-video-replication) —— 复制爆款
- [x-viral-video-breakdown](https://github.com/kkone1238899/x-viral-video-breakdown) —— 拉片
- [x-viral-video-de-ai](https://github.com/kkone1238899/x-viral-video-de-ai) —— 去 AI 味
- [x-viral-video-characters](https://github.com/kkone1238899/x-viral-video-characters) —— 人物构建
- [x-viral-video-editing](https://github.com/kkone1238899/x-viral-video-editing) —— 视听剪辑技巧
- [x-viral-video-prompt-opt](https://github.com/kkone1238899/x-viral-video-prompt-opt) —— 提示词优化
- [x-viral-video-copywriting](https://github.com/kkone1238899/x-viral-video-copywriting) —— 文案
- [x-viral-video-showcase](https://github.com/kkone1238899/x-viral-video-showcase) —— X 病毒视频合集

## 投稿

发现好的流水线 / 生产管线 prompt / skill，欢迎提 Issue 或 PR（格式见 CONTRIBUTING.md）。

## 更新日志

- 2026-10-12：6 个项目条目按铁律升级（表格→小节：补核心用法 / 常见坑 / 适用场景 / 来源，Star 数与更新时间重验）
- 2026-10-11：首版，6 个项目，持续收录中
