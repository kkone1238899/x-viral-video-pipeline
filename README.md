# 流水线 / 生产管线

> 一条视频做一下午？这个库收集一句话到成片的自动化生产管线，每条都写清楚能帮你解决什么、怎么用它搞钱。
>
> A curated collection of production pipelines prompts & skills for viral short videos, gathered from practitioners sharing on X.
> 
> Each entry answers two questions: what problem it solves (and who it's for), and how to make money with it.
> 
> Star counts verified via GitHub API on 2026-10-21. Continuously updated.

## 条目

### Huobao Drama（chatfire-AI/huobao-drama）

**核心提炼**
- 解决什么问题：一句话或一部小说进去，剧本→角色设计→分镜拆分→成片合成，整条短剧流水线在一个平台里走完；四个内置 Agent 分别负责小说改剧本、抽取角色/场景/道具、分镜拆分、生成生图/生视频提示词。
- 核心用法（4 步）：1) 下载桌面版（macOS / Windows）或 Docker 部署；2) 在「设置」里填入模型 API Key（一键写三个常用配置）；3) 新建项目，输入一句话或小说，Agent 自动完成角色设计和分镜拆分；4) 逐集检查确认后，合成整集导出成片。
- 什么时候用 / 常见坑：适合想从 0 搭短剧生产工作室、批量出剧的人；协议为 CC BY-NC-SA 4.0（非商业），拿它接单前先看清授权；需要自备文本 / 图像 / 视频三类模型 API。

**适用场景**：短剧团队、内容工作室、想批量产出短剧的创业者。

**怎么用它搞钱**：短剧批量生产 / 小说推文。

**来源**：[chatfire-AI/huobao-drama](https://github.com/chatfire-AI/huobao-drama) · ⭐16453 · 更新于 2026-10-21

### AutoClip（zhouxiaoka/autoclip）

**核心提炼**
- 解决什么问题：把播客、访谈、课程等长视频自动剪成短视频，一并生成字幕、封面和发布文案，适配抖音、小红书、TikTok、Reels、YouTube Shorts。
- 核心用法（4 步）：1) 下载桌面版（安装包自带 Python 和 FFmpeg，免配环境）；2) 在设置里选模型服务商、填 API Key 并测试连接；3) 贴一个长视频链接，选好平台版式；4) 预览自动成片，检查字幕和取景后下载发布包或直发。
- 什么时候用 / 常见坑：做课程切片、知识博主矩阵号时用；软件免费、云端模型按量计费，量产前先算清费用；Intel Mac / Linux 建议走 Docker 或 CLI 版。

**适用场景**：知识付费从业者、课程切片代运营、要做多平台分发的人。

**怎么用它搞钱**：知识付费 / 课程切片代运营。

**来源**：[zhouxiaoka/autoclip](https://github.com/zhouxiaoka/autoclip) · ⭐9601 · 更新于 2026-10-21

### Jellyfish（Forget-C/Jellyfish）

**核心提炼**
- 解决什么问题：AI 短剧的端到端生产工作台——脚本理解、分镜拆分、角色/场景/道具/服装一致性管理、镜头级生图生视频、异步任务跟踪都在一个界面里，专治"换镜头人物就变脸"。
- 核心用法（4 步）：1) 用 Docker Compose 起前后端服务；2) 导入剧本，AI 拆镜头并抽出角色、场景、道具、服装；3) 为每个镜头准备候选素材（人物图、关键帧），确认状态变为 ready；4) 生成镜头级视频并导出。
- 什么时候用 / 常见坑：短剧已经有一定产量、一致性问题开始拖慢交付时用；它本质是偏生产管理的自建工具，需要自己准备服务器和模型。

**适用场景**：短剧工作室、想把短剧流程工具化的制作团队。

**怎么用它搞钱**：短剧工作室降本接单。

**来源**：[Forget-C/Jellyfish](https://github.com/Forget-C/Jellyfish) · ⭐6791 · 更新于 2026-10-20

### Automate Faceless Content（cporter202/automate-faceless-content）

**核心提炼**
- 解决什么问题：一份"无真人出镜内容自动化"的完整课程指南（10 个模块，4–6 周课表），从入门、工具配置、选题脚本做到变现和规模化，按步带新手做出第一条无出镜视频。
- 核心用法（4 步）：1) 读 Getting Started 指南，了解无出镜内容的逻辑；2) 按 Account Setup 注册并配置生成工具；3) 跟着 Your First Video 做出第一条视频；4) 按 Monetization 章节逐个平台开通收益（YouTube 收益、联盟营销等）。
- 什么时候用 / 常见坑：适合零基础、想按课表学完的人；它深度绑定自家商业工具 ViralWave Studio（有免费试用），工具推荐偏向它家——介意绑定的话，只取课程框架和方法论。

**适用场景**：零基础想做 YouTube / TikTok 无出镜账号的人。

**怎么用它搞钱**：养生 / 故事号矩阵。

**来源**：[cporter202/automate-faceless-content](https://github.com/cporter202/automate-faceless-content) · ⭐3170 · 更新于 2026-10-20

### AI Faceless Video Generator（SamurAIGPT/AI-Faceless-Video-Generator）

**核心提炼**
- 解决什么问题：输入一个话题，自动生成脚本、配音，再用 SadTalker 让一张人脸图"说话"，一条流程跑完就是一条口播视频，全程不用真人出镜。
- 核心用法（4 步）：1) 在 Colab 里打开官方笔记本（官方推荐，省去本地配 GPU）；2) 填入 OpenAI API Key；3) 输入话题和一张人脸图（可用任意头像）；4) 跑完全部 cell，下载成片。
- 什么时候用 / 常见坑：想快速验证口播选题时用；需要 OpenAI API Key，SadTalker 对 GPU 有要求（走 Colab 可绕过）；配音走 gTTS，中文号先跑一条试听再决定。

**适用场景**：想快速测试口播选题的个人创作者、口播号代做。

**怎么用它搞钱**：口播号代做。

**来源**：[SamurAIGPT/AI-Faceless-Video-Generator](https://github.com/SamurAIGPT/AI-Faceless-Video-Generator) · ⭐521 · 更新于 2026-10-20

### Lingjian Video / 灵剪（dososo/blcaptain-lingjian-video）

**核心提炼**
- 解决什么问题：一句话生成发布级中文短视频（脚本、配音、画面、配乐、字幕、音效全自动），但和黑箱出片相反——脚本、配音、画面三关都停下来给你审，逐关确认才继续。
- 核心用法（4 步）：1) 本地运行，配好 LLM、语音和画面模型 Key（`doctor` 会告诉你缺什么、怎么补）；2) 一句话说清目标（平台、主题、比例、内容依据）；3) 逐关确认：脚本关挑版本 → 配音关试听选音色 → 画面关看分镜确认单，每关点头才进下一关；4) FFmpeg 渲染，QA 全绿后导出多平台分发包。
- 什么时候用 / 常见坑：接客户商单、对成片质量有要求、怕黑箱返工时用；它是 CLI / agent 驱动的工程工具，需要一定技术动手力；审批用签名绑定产物内容，内容一改批准自动失效（防偷工减料，也是改一句就要重审整关的代价）。

**适用场景**：接商单的视频创作者、本地商家探店代运营、有技术动手力的个人。

**怎么用它搞钱**：本地商家探店代运营。

**来源**：[dososo/blcaptain-lingjian-video](https://github.com/dososo/blcaptain-lingjian-video) · ⭐254 · 更新于 2026-10-17

### AutoVio（Auto-Vio/autovio）

**核心提炼**
- 解决什么问题：大多数 AI 工具只管视频制作的一个环节，AutoVio 把整条链路跑完——一句话进去，LLM 写分镜脚本、逐场景生图、生图转视频片段、时间线编辑器组装、导出 MP4，全程自托管。
- 核心用法（4 步）：1) 自托管部署（TypeScript/React/Express/MongoDB 全栈）；2) 在 Init 里设定主题、受众、分辨率和可选参考素材；3) 可选上传参考视频，视觉 AI 提取风格、节奏、配色（Analyze）；4) 走完 Scenario→Generate→Editor 五步流程（文档齐全），导出成片。
- 什么时候用 / 常见坑：适合 SaaS 产品演示、功能官宣、营销视频的团队和开发者；生图/生视频的模型 Key 自备（Gemini/DALL-E 生图、Veo/Runway 生视频）；协议为 PolyForm Noncommercial（非商业），商用前先看清授权；MCP-ready，可被 agent 直接调用。

**适用场景**：SaaS 团队、开发者、要批量做产品演示 / 营销视频的人。

**怎么用它搞钱**：产品演示视频代做 / SaaS 营销视频接单。

**来源**：[Auto-Vio/autovio](https://github.com/Auto-Vio/autovio) · ⭐33 · 更新于 2026-10-17

### Video Generation Workflow Skill（NickQi688/video-generation-workflow）

**核心提炼**
- 解决什么问题：中文 skill，把"一句话视频需求 / 一篇实操文章 / 一个产品介绍"变成可执行的视频生产流程——核心不是写一个视频 prompt，而是像视频制作项目经理一样工作：边问边定方向（目标、风格、画幅），边拆边执行（脚本、分镜、口播稿、字幕稿、视觉预演图 prompt）。
- 核心用法（4 步）：1) clone 到 Codex skills 目录（`~/.codex/skills/video-generation-workflow`）；2) 在 Codex 里调用，skill 先问清目标和风格，并让用户选画幅（16:9 横版 / 9:16 竖版 / 1:1 方版）；3) 产出分镜表、口播稿、字幕稿、视觉预演 prompt；4) 指导 Codex 用 HyperFrames / Remotion / HTML / React 代码驱动生成可渲染场景并导出视频。
- 什么时候用 / 常见坑：适合把实操文章改教程视频、产品介绍改演示视频、工具教程改小红书 / 抖音 / YouTube 视频；给客户先出视频方案、再按反馈逐镜头微调时好用；是 skill 形态，需要配 Codex / Claude Code 类 agent 环境；暂无 LICENSE，商用前注意授权风险。

**适用场景**：知识博主、产品 / 工具创作者、接视频方案商单的人。

**怎么用它搞钱**：知识教程视频代做 / 产品演示视频商单。

**来源**：[NickQi688/video-generation-workflow](https://github.com/NickQi688/video-generation-workflow) · ⭐60 · 更新于 2026-09-07

### Remotion Idea to Video（coleam00/archon-video-generation-workflow）

**核心提炼**
- 解决什么问题：一条 Archon 工作流，把任意 URL 或一句话变成带配音的短视频——自动抓取 Hacker News 今日热帖或指定文章 / 产品页，生成讲解 / 营销视频，用 Remotion 渲染成 mp4 并按日期归档进仓库，Studio 里可回看全部历史成片。
- 核心用法（4 步）：1) 按 README 让 coding agent（Claude Code 优先，也支持 Codex / Pi）把仓库跑到可运行；2) 选 TTS 服务商（Cartesia 或 ElevenLabs）并填 Key；3) 传 mode 调用：`hn`（今日 HN 热帖自动成片）、`article <url>`（文章转讲解视频）、`marketing <url>`（产品页转 pitch 视频）、`idea <prompt>`（一句话主题）；4) 每次运行在 `src/<CompId>/` 落新 composition，mp4 进 `./videos/<date>-<slug>/`。
- 什么时候用 / 常见坑：适合做"热点速报 / 文章转视频"的日更号；README 是写给 agent 看的单一事实源，按步骤走即可；需要 coding agent 环境 + TTS Key；暂无 LICENSE；21★ 刚过收录线，社区验证尚浅，先跑一条验证再量产。

**适用场景**：热点资讯号、文章转视频的内容创作者、技术博主。

**怎么用它搞钱**：热点速报号日更 / 文章转视频代运营。

**来源**：[coleam00/archon-video-generation-workflow](https://github.com/coleam00/archon-video-generation-workflow) · ⭐21 · 更新于 2026-10-02

### X 实战帖 · 核心提炼

> 以下条目均已提炼：不点链接也能拿走 80% 干货，原帖链接只做署名出处。

### @techniqco：企业级 YouTube Shorts 生产管线——n8n 编排，单条成本约 $0.48

**核心提炼**
- 解决什么问题：想跑 YouTube Shorts 频道但每条都手工做太慢——这条英文线程给了一条"企业级"全自动管线：n8n 编排，GPT-4o-mini 写脚本，ElevenLabs 配音，Creatomate 渲染，YouTube API 自动发布；50 秒短视频单条成本 $0.37–$0.59。
- 核心用法（4 步）：1) 按线程里的 n8n starter 模板导入工作流（可直接下载）；2) 接入 GPT-4o-mini（脚本）、ElevenLabs（配音）、Creatomate（渲染）三家的 Key；3) 设定选题和发布节奏，管线自动跑完脚本→配音→渲染→发布；4) 用 YouTube API 把发布也收进管线，定时自动上线。
- 什么时候用 / 常见坑：适合做英文 Shorts 矩阵、想把"做号"变成无人值守流水线的人；成本大头在配音和渲染两家 API，先用模板跑一条测真实账单；n8n 模板是英文生态，中文号要换配音和脚本链路。

**适用场景**：YouTube Shorts 矩阵号、想做无人值守英文短视频频道的人。

**怎么用它搞钱**：英文 Shorts 矩阵跑广告分成 / 把这套管线打包成代运营服务。

**来源**：[@techniqco](https://x.com/techniqco/status/2110304510426124602) · 2026-10-14

### @Chenfacai0（陈发财）：Toonflow——「AI 短剧流水线」，剧本输入即出成片

**核心提炼**
- 解决什么问题：短剧制作环节多、人工串起来慢——Toonflow 是开源 AI 短剧/漫剧创作平台：剧本输进去，分镜、角色、视频三层 Agent 并行干活，直接出成片；无限画布 + AI Agent + 可视化工作流，本地部署、自选模型。
- 核心用法（4 步）：1) 本地部署（支持跨平台客户端，MCP 与插件可扩展）；2) 输入剧本，平台做智能分镜、角色与场景资产管理；3) 三层 Agent 并行：分镜层排镜头、角色层锁一致性、视频层生画面；4) 图像生成→视频生成→成片导出。
- 什么时候用 / 常见坑：适合想自己搭短剧生产工作室、数据要私有化的人；评论区实测成本参考：本地跑约 50 元/分钟，成本大头在视频模型调用——同一剧本换模型账单能差数倍，量产前先拿一集测各家模型；项目 18670★、MIT 协议，当日仍在更新。

**适用场景**：短剧/漫剧工作室、想私有化部署 AI 视频管线的人。

**怎么用它搞钱**：短剧批量生产接单 / 漫剧推文号矩阵。

**来源**：[@Chenfacai0](https://x.com/Chenfacai0/status/2112687305920033024) · 项目：[HBAI-Ltd/Toonflow-app](https://github.com/HBAI-Ltd/Toonflow-app)（⭐18670 · MIT · 更新于 2026-10-21）

### @xoyif63862452（北衡）：Agent 做视频——7 套现成 Skills 的选型地图

**核心提炼**
- 解决什么问题：Agent 做视频的 Skills 太多不知道怎么选——这篇把方法论和选型一次讲透：Claude Code/Codex 类 Agent 接 Skill，把视频制作拆成可执行流水线（分析参考片、生成分镜、剪素材、做动画、批量改文案、自动渲染）；起步建议从最烦的环节切入（转写、粗剪、字幕、模板动画）。
- 核心用法（7 套盘点 + 选型建议）：OpenMontage（12 条流水线/100+ 工具/700+ Skill 文件，偏全流程）；HyperFrames（HTML+data 属性→Puppeteer 截图→FFmpeg 合成，`npx skills add heygen-com/hyperframes`，偏代码驱动）；Hypit（爆款视频拆成可编辑工作流，一条内容批量生成一百个变体，擅长拆爆款）；video-use（转写+关键帧截图→模型判断剪辑点→EDL 时间线，适合播客切片/Vlog 整理）；Claude Code Video Toolkit（配音/生图/配乐/数字人/Remotion 合成，走 Modal/RunPod 云 GPU）；MoneyPrinterTurbo（主题自动生成文案/字幕/配音合成视频，适合批量短视频）；Remotion Skills（React 写视频，偏代码驱动）。
- 什么时候用 / 常见坑：先装一套跑通再叠加，别一次全装；OpenMontage 已在编剧/脚本库收录，不重复计入。

**适用场景**：想用 Agent 搭视频生产管线、但不知从哪个 Skill 下手的人。

**怎么用它搞钱**：按这张选型地图给客户搭管线做代建服务 / 批量短视频代运营。

**来源**：[@xoyif63862452](https://x.com/xoyif63862452/status/2112704313256477111) · 文章：[Agent 做视频：7 套现成 Skills 直接抄作业](https://x.com/i/article/2112703334167859200) · 2026-10-21

### @qinghaiwu9527（盈盈）：WorkBuddy + 漫剧智能体团队——3700 字小说自动跑完分镜

**核心提炼**
- 解决什么问题：漫剧制作六道工序（大纲→角色→美术→剧本→分镜→出图）人工接力慢——这套在 WorkBuddy 里搭"六名执行角色 + 一名总调度"的智能体团队，3700 字小说从大纲一路推到分镜，全套资产设计自己跑完。
- 核心用法（4 步）：1) 装开源技能包 eternityspring/shuohao-skills（4883★、Apache-2.0，Node 18+、无 npm 依赖）；2) 上传小说，六个技能按工序自动接力：novel-outline（短剧大纲五件套，14 道质量门）→ novel-characters（角色形象+音色提示词）→ novel-art（场景道具美术设定，10 道门）→ novel-script（场次节拍流+时长折算，10 道门）→ novel-storyboard（分镜图，直出 H3 和 Seedance 投产包，18 道门）→ character-refs（出图，支持 Qwen/codex/GPT Image）；3) 质量门自动把关，不合格打回；4) 用 Seedance 生成视频（1080P 2 秒/积分、720P 3 秒/积分，3700 字小说全部视频约 150 积分）。
- 什么时候用 / 常见坑：适合做漫剧/短剧、想把"资产设计"环节自动化的团队；想 0 积分跑通也有三条路：ComfyUI+ControlNet、开源视频模型本地部署、Kling 每日免费额度；直出 H3/Seedance 投产包是亮点，MiniMax H3 用户优先。

**适用场景**：漫剧/短剧团队、小说推文号、想自动化资产设计环节的人。

**怎么用它搞钱**：漫剧批量生产 / 小说推文号矩阵。

**来源**：[@qinghaiwu9527](https://x.com/qinghaiwu9527/status/2112460724043964697) · 文章：[0积分!我用 WorkBuddy + HY3 搭了个AI漫剧智能体团队2.0](https://x.com/i/article/2112367747854454784) · 2026-10-20

### @justloveabit（loveabit）：写 HTML 出视频——HyperFrames 爆款短视频流水线实操

**核心提炼**
- 解决什么问题：AI 生视频贵且不可控——HyperFrames 是"Write HTML, Render Video"的开源框架（68514★、Apache-2.0），让 Agent 写 HTML 生成视频：标题淡入、背景缩放、数据柱状图、口播字幕全是代码，改一行字就是改一版视频。
- 核心用法（4 步）：1) 装 skill：`npx skills add heygen-com/hyperframes`；2) 给 Agent 一句话需求（如"10 秒产品介绍视频"），它写出带标题淡入、背景缩放、数据柱状图、口播字幕的 HTML；3) 三类场景有现成 Prompt 模板：产品类（15 秒竖版：标题淡入、背景动态模糊、价格按钮动画）、数据类（CSV 柱状图竞赛动画 30 秒，配解说字幕）、口播类（竖版动态字幕，60 秒内）；4) 本地渲染出片，15 分钟出第一条成片。
- 什么时候用 / 常见坑：适合产品介绍、数据可视化、口播类短视频；省钱链路：本地渲染 + 本地 TTS（如 Kokoro）+ 本地图片生成，整条链路几乎零成本；它是代码驱动路线，画面靠排版和动画，拍不了真人实拍质感。

**适用场景**：产品/工具创作者、数据博主、想低成本批量出短视频的人。

**怎么用它搞钱**：产品介绍视频代做 / 数据可视化短视频接单。

**来源**：[@justloveabit](https://x.com/justloveabit/status/2111682519796166979) · 项目：[heygen-com/hyperframes](https://github.com/heygen-com/hyperframes)（⭐68514 · Apache-2.0 · 更新于 2026-10-21）

### @zhu185178（Feicai）：Opus 5.5 当导演——开源工作流「广告分镜师」完整实战

**核心提炼**
- 解决什么问题：AI 广告片"导演"环节缺方法论——这套开源工作流 feicaiclub/ad-storyboarder（MIT）装在 Claude Code 里，Opus 5.5 当导演兼制片，接 Higgsfield（主力 Seedance 2.5）生成画面和声音；附带完整实战：给特斯拉 Roadster 做 41 秒概念广告，从开工到交第二版不到 6 小时。
- 核心用法（4 步）：1) 把工作流装进 Claude Code，六个 Skill（拷问需求、脚本、参考、生成、剪辑、自审）可单独调用；2) 主控只写 6 件事：需求问透、脚本定稿、参考齐全、每段过审、成片过门禁、交付——只在超预算/删文件/对外发布/动账号时停下来问人；3) 脚本拆段（本例 14 段、每段 1–5 镜头），美术资产全由 Agent 自备，先 480p 试拍开场再铺开；4) 只读审片员逐条抽帧查连戏（本例第一版挑出 6 处必须改），Studio 插件（/ad-studio）按时间码标记问题帧，第二版左右并排对照。
- 什么时候用 / 常见坑：七个实战技巧——不再手写提示词（沟通内容即项目上下文）；没有万能模型（人像用 Seedream/Nano Banana Pro/Midjourney，视频用 Seedance 2.5）；先 480p 试拍（5 秒镜头 1080p 80 积分 vs 480p 15 积分）；参考图要干净纯色背景；一定要有另一个 AI 当审片员；少用关键帧；运镜对了就别改提示词——剪辑是最便宜的修法。成本账：本例开工 1753 积分，两版交完剩 1.82；项目仅 7★ 刚开源，先跑通再量产。

**适用场景**：接广告/宣传片商单、想用 Agent 跑完整制作流程的创作者。

**怎么用它搞钱**：广告概念片代做 / 汽车/产品品牌方商单。

**来源**：[@zhu185178](https://x.com/zhu185178/status/2112127321905762500) · 文章：[我用 Opus 5.5 做了一条广告，这是完整教程](https://x.com/i/article/2112124221845598208) · 2026-10-19

### @Steel_web（Sophie_404）："agents make the thing that makes the video"——Claude Code 代码驱动动效管线

**核心提炼**
- 解决什么问题：传统动效制作困在时间线+关键帧里，改一版就要重新调渲染——这套"代码驱动"管线把视频制作变成写代码：Claude Code 当导演兼动画师，视频引擎+动画库+Blender 当渲染农场，"睡觉时也在渲染"。
- 核心用法（4 步）：1) 准备一个文件夹：spec.md（场景规格）+ assets/（素材）+ render.py（渲染入口）；2) 把文件夹交给 Claude Code，配好视频引擎、动画库、Blender；3) Claude 写场景（scene），引擎逐帧渲染，ffmpeg 合成音频；4) 要改版？直接改代码——"the edit is a git diff"，没有时间线、没有关键帧。
- 什么时候用 / 常见坑：适合动态图形/信息可视化/产品演示类视频，拍不了真人实拍质感；这是方法论分享帖（附 25 秒实拍演示视频），没有开源仓库——照着搭需要自己备齐引擎和 Blender；英文原帖，核心概念已提炼。

**适用场景**：动态设计师、想把"改稿"变成"改代码"的视频创作者、有代码动手力的人。

**怎么用它搞钱**：动态图形/数据可视化视频代做 / 把"agent 渲染农场"打包成工作室服务。

**来源**：[@Steel_web](https://x.com/Steel_web/status/2112802429821678034)（线程共 3 帖：25 秒演示视频 + 方法论 + 技术栈）· 2026-10-21

### @drahcir_rahl：Hermes Agent 端到端视频工具链——非视频专业者的开箱方案

**核心提炼**
- 解决什么问题：不是视频专业出身的人，面对一堆 AI 视频工具不知道怎么串成完整流程——这套 toolchain 把"常用的 agentic 工具"编排成一套端到端方案，让非专业的人也能跑完"采集→制作→后期"全流程。
- 核心用法（3 段架构，按仓库描述）：1) OpenScreen capture（录屏/采集）；2) HyperFrames authoring（HTML 代码驱动出片，库内已有 HyperFrames 条目可对照）；3) headless post-processing（无头后期处理）；三段"wired into one skill"——装成一个 skill，Agent 直接调用。
- 什么时候用 / 常见坑：适合想给自家 Agent 配"一键出视频"能力的开发者；仓库刚开源（1★、2026-10-20 更新），社区验证尚浅，先跑通再量产；仓库暂无明确 LICENSE，商用前注意授权；Shell 脚本形态，需要一定动手力。

**适用场景**：想给 Agent 加视频生产能力的开发者、非视频专业的 AI 创作者。

**怎么用它搞钱**：Agent 视频能力代建 / 非专业客户的"一键出片"服务。

**来源**：[@drahcir_rahl](https://x.com/drahcir_rahl/status/2112786295386693787)（线程 1/，附 150 秒演示视频）· 项目：[rahlquist/hermes-video-toolchain](https://github.com/rahlquist/hermes-video-toolchain)（⭐1 · 更新于 2026-10-20）· 2026-10-21

### @yuanliuwei（袁六伟｜一人AI公司）：暗黑数据科普视频 Skill——6 步流水线，B站百万播放款可复刻

**核心提炼**
- 解决什么问题：深黑底+橙红光晕+数字滚动的"暗黑数据可视化"科普片（B站动辄百万播放），过去要手绘+剪辑——这套 Skill 让 WorkBuddy/Codex/Claude 直接跑完：选题准入→找数据→脚本分章→场景部件→渲染配乐→质检，6 步全写在 Skill 里。
- 核心用法（6 步）：1) 选题三准入：有认知反差（"你以为 A，其实 B"）、有可查权威数据、无合规风险；2) 每章配真实数字，标机构/年份/样本量；3) 先写分镜时间表再写代码，铁律"每章时长=动画走完时间+0.8 秒"，样片因此只有 27 秒；4) 10 种场景部件按数据类型选（占比用圆环、对比用柱状图、趋势用曲线）；5) 先渲静帧检查→按 CPU 核数切 8 段并行渲染→ffmpeg 拼接（813 帧/8 核 Linux 不到 1 分钟）；6) music_gen_v2.py 生成原创氛围音（中频适配手机外放）→preflight.py 一次质检分辨率/码率/峰值/首帧封面。
- 什么时候用 / 常见坑：适合保险/健康/理财/教育等"有普遍误解+有权威数据"的行业；只依赖 ffmpeg/Pillow/numpy，不用商业视频软件；Linux 中文字体坑：font_finder.py 自动探测 Noto Sans CJK，ttc 简体中文在 index 2；保险理财强监管：只做科普不承诺收益；仓库今日刚开源（0★），先跑通再量产。

**适用场景**：保险/健康/理财从业者、知识科普号、想批量做数据可视化短视频的人。

**怎么用它搞钱**：保险/理财知识科普获客 / 数据可视化短视频代做。

**来源**：[@yuanliuwei](https://x.com/yuanliuwei/status/2112795034235834677) · 文章：[爆火的暗黑数据科普视频，Workbuddy/codex 轻松复刻](https://x.com/i/article/2112793728196694016) · 项目：[sixwei2025/dark-infographic-video-skill](https://github.com/sixwei2025/dark-infographic-video-skill)（⭐0 · MIT · 更新于 2026-10-21）· 2026-10-21

### @yuanliuwei：全网爆火的 Vibe 知识大赏，保姆级复刻教程

**核心提炼**
- 解决什么问题：上线 12 天 6 亿播放的"Vibe 知识大赏"（代码一帧帧画出来的知识动画）——这篇把复刻拆成可执行的保姆级 7 步：装进 Agent（WorkBuddy/Codex/Claude Code）→别急着写代码（先读 SKILL.md，题目到成片 9 步）→写分镜表→先拼图再渲染（--sheet 截帧拼图、--motion 抽 12 帧看转场，"至少改两轮再给用户看"）→渲染和配声音（--det 确定性自检、--jobs 4 四路并行；42 秒片子 3 分钟出完；audio.py 自动合成音效；输出 1920×1080/30 帧/带声 MP4）。
- 最值钱的一句："配图不是讲解"——翻车案例：第一版《折叠》讲蛋白质全片是星点折线，换任何文案都成立=配图；重做后镜头钻进红细胞找到一串珠子=讲解。字幕要被"演"出来（说"砍掉一半"屏上真盖住一半）；每个概念找一个认得的形象（一串珠子/红细胞/尺子/纸）。
- 什么时候用 / 常见坑：适合知识博主/一人公司/老师做 1–3 分钟横屏知识片；三次踩坑：python→python3、PEP 668→建 venv；依赖 playwright/numpy/scipy/Pillow/本机 Chrome/ffmpeg/SIL OFL 字体；仓库 484★（2026-10-13 更新），暂无明确 LICENSE，商用前注意授权；样片《折纸到月亮》42 秒，地月 384,400km（NASA）。

**适用场景**：知识博主、一人公司（产品原理介绍片）、老师（课前 30 秒概念片）。

**怎么用它搞钱**：知识动画视频代做 / 企业产品介绍片商单。

**来源**：[@yuanliuwei](https://x.com/yuanliuwei/status/2112799690911515041) · 文章：[全网爆火的 Vibe 知识大赏，保姆级教程](https://x.com/i/article/2112791105926279168) · 项目：[Dave-cc/vibe-knowledge-film](https://github.com/Dave-cc/vibe-knowledge-film)（⭐484 · 更新于 2026-10-13）· 2026-10-21

### @yuanliuwei：用 Grok Bot 打造了一个短视频工作室，0 成员

**核心提炼**
- 解决什么问题：一个人如何撑起可控的短视频分发产能——7 条专线 Bot 矩阵：实验室探路 + 操盘手 1–6（心理/文哲/短剧/3D 地图/口播/宣传片）量产；人只回"是/否"验收成片，"人睡觉机器出片"。
- 四条硬产线（只写可核对的）：心理线——15–30 秒无人声纯字幕新风格，JSON 驱动 Remotion 产线；2026-10-20 一次排 10 条进抖音创作者中心定时发布，自动填标题/话题/挂配乐/勾 AI 生成声明；选题库 CSV 313 行。口播线——选题→口播稿→分镜→Voicebox 克隆声→逐字字幕→Mac 渲染→首帧封面→质检→桌面交付；upload_draft.py 连视频号助手自动发表。3D 地图线——MapLibre 三维地形+无头 Chrome 逐帧+ffmpeg；桌面 8 条 mp4，视频号"山河来电"已核实发出 4 条。宣传片线——武汉"一天时间线"电影航拍：18 关键帧→18 段动态镜头→约 80 剪辑点→Voicebox 克隆声，全程无人手剪。
- 组织方法：实验室先测形式、测通沉淀给操盘手量产；各操盘手维护"当前状态.md"；作者诚实边界：只写可核对的成片数/发出数，不编播放量涨粉曲线。
- 什么时候用 / 常见坑：适合想搭"0 员工短视频工作室"的一人公司/小团队；4 个 Skill 仓库均为今日开源（0★、MIT）：psych-kepu / 3d-map / dark-infographic / talking-head（均为 sixwei2025），先跑通再量产。

**适用场景**：一人公司、小团队、想自建分发产能的企业。

**怎么用它搞钱**：企业短视频代运营（城市宣传片/skill 交付/客户内容产能）/ Bot 矩阵方法论咨询。

**来源**：[@yuanliuwei](https://x.com/yuanliuwei/status/2112794126693396647) · 文章：[用Grok Bot打造了一个短视频工作室，0 成员](https://x.com/i/article/2112792268432199680) · 2026-10-21

### @yuanliuwei：爆火的心理科普视频，Workbuddy/codex 轻松复刻

**核心提炼**
- 解决什么问题：心理科普是长期流量（喵的心理课《泪失禁》449.9 万赞/109.6 万分享）+离成交近（壹心理 5300 万+用户）——这套 Skill 把 15–30 秒心理科普片做成 5 步流水线，WorkBuddy/Codex 可跑。
- 核心用法（5 步）：1) 选题：从人性母题出发（好奇与窥探/焦虑与安全感/控制感），挑多个账号反复做爆过的题，只留能用"一个机制"讲清的；2) 脚本分镜：只讲一件事、一种情绪，不给解决方法；钩子/现象/核心机制/互动题四段；结尾"你是 1 还是 2"选择题拉互动；3) 动画渲染：Remotion 代码化，第 0.01 秒插 3:4 竖屏大字封面，导出 1920×1080 静音成片；4) 抽帧自检：每秒抽一帧对清单查时长/封面/字幕/配色；5) 定时发布：挂 BGM、勾 AI 生成声明。人只做两件事：定选题、最后看一眼成片。
- 什么时候用 / 常见坑：适合心理/情感/成长赛道；"代码能复用=能批量"，需求大+能承接+可批量才值得做；仓库今日开源（0★、MIT）；作者声明：数据为 2026-10 公开页面所见，不承诺播放结果。

**适用场景**：心理/情感博主、心理服务机构、想批量做科普动画的人。

**怎么用它搞钱**：心理科普号矩阵 / 心理机构内容代运营（短视频是服务平台入口）。

**来源**：[@yuanliuwei](https://x.com/yuanliuwei/status/2112793414618038389) · 文章：[爆火的心理科普视频，Workbuddy/codex 轻松复刻](https://x.com/i/article/2112790294038994944) · 项目：[sixwei2025/psych-kepu-video-skill](https://github.com/sixwei2025/psych-kepu-video-skill)（⭐0 · MIT · 更新于 2026-10-21）· 2026-10-21

### @justloveabit（loveabit）：一句话让 Coding Agent 给你做 30 秒商业级产品宣传片

**核心提炼**
- 解决什么问题：给新产品做 30 秒宣传片，外包动辄几千上万、自己啃 AE 改个字要重导——huashu-motion Skill 装进 Coding Agent（Claude Code/Codex），丢一句"帮我给这个项目做个 30s 发布片"，全自动完成剧本→动效→配乐。
- 最绝的"指着画面改"：浏览器里所见即所得——标题字号小直接拖拽缩放、换主题色吸管一点全局更新、节奏不对时间轴拖关键帧；改完即时导出 4K/60fps 无损 MP4。
- 什么时候用 / 常见坑：适合独立开发者/一人公司的产品发布片；仓库 1194★、MIT（2026-10-19 更新），社区验证充分；环境要求 Node 22+、本机 Chrome 和 FFmpeg，作者称目前只在 macOS 实测；Codex 沙箱会拦本地预览和浏览器（评论区 @DotsonZion 实测）。

**适用场景**：独立开发者、一人公司、要频繁出产品宣传片的人。

**怎么用它搞钱**：产品发布片代做 / 独立开发者宣发服务。

**来源**：[@justloveabit](https://x.com/justloveabit/status/2112743359827902807)（附 GIF 演示）· 项目：[alchaincyf/huashu-motion](https://github.com/alchaincyf/huashu-motion)（⭐1194 · MIT · 更新于 2026-10-19）· 2026-10-21

### @xiaohu（小互）：XiaoHu AI 日报的视频版 Demo——Claude Code 全流程自动跑

**核心提炼**
- 解决什么问题：@小互（12.6 万粉）把自家 AI 日报做成视频版 Demo：内容抓取→动画效果→视频制作→剪辑，全由 Claude Code 自己完成；固定模板后可自动化，甚至每小时跑一次。
- 什么时候用 / 常见坑：适合资讯/日报类账号的视频化；动态模板与指导来自 @lemomo_ai；下一步是解决声音拟真（更像真人）；这是 Demo 验证可行性——模板+定时=无人值守资讯视频号。

**适用场景**：资讯博主、日报/周报类账号、想做自动化视频资讯的人。

**怎么用它搞钱**：资讯视频号矩阵 / 企业资讯视频代运营。

**来源**：[@xiaohu](https://x.com/xiaohu/status/2112748049609158836)（附 3 分钟演示视频）· 2026-10-21

### @lisenhai9999（AI搞钱小海）：我用 AI 做 YouTube Shorts，一个月赚了 1200 美金

**核心提炼**
- 解决什么问题：一条可复制的英文 Shorts 批量管线+真实收益账：GPT 生成冷知识文案（一天 10 条）→ElevenLabs 英文配音→Pika 生成画面→上传 YouTube 挂广告；标题用 AI 优化，点击率翻倍；首月 $200→第三个月稳定 $1500 左右。
- 什么时候用 / 常见坑：适合做英文科普/冷知识 Shorts 矩阵；赛道选择逻辑：冷知识"永远有流量"；该账号今日多条同模板 AI 生成内容，此篇因步骤/工具/产能/收益数据完整而收录——收益数字为作者自述，入库时自行权衡；Pika/ElevenLabs 均为付费 API，量产前先算账。

**适用场景**：想做英文 Shorts 矩阵赚广告分成的人。

**怎么用它搞钱**：英文 Shorts 矩阵跑广告分成 / 把这套管线做成代运营服务。

**来源**：[@lisenhai9999](https://x.com/lisenhai9999/status/2112796777346638262) · 2026-10-21

### @aisongman（AiSongMan｜AI Workflow Lab）：完全自動 MV 作成ワークフロー——Claude Code 当导演

**核心提炼**
- 解决什么问题：Claude Code 当"导演"，1 分钟男女对唱 MV（2K、带唇形同步）全自动跑完——人只做看片+指出修改点，一次没自己写过 prompt。
- 核心用法（6 步）：⓪ 人给曲+方向（"日系MV×K-POP感、男女2人、无舞蹈、1 分钟副歌结束淡出"）；① Claude 解析曲子（BPM/节拍/副歌位置；UVR 分离人声→Whisper 取歌词时间轴）；② Higgsfield 生成角色设定+分镜关键帧；③ MiniMax H3 参考视频生成（关键帧+角色图+人声参考做唇形同步；试作本机 ComfyUI 720p，正式 Higgsfield 2K；全片 18 镜/232 credits）；④ Claude 全片质检重做（运镜数值化、唇形按音程自动补正、NG 镜重拍）；⑤ Remotion 剪辑（卡 beat 剪辑、歌词 motion、副歌闪卡）；⑥ 人验收。
- 三个实战学：歌词转写先分离人声精度更高；运镜必须明写（orbit/crane/dolly），否则=静止画 zoom；参考图写"场所/光的参考"别写"按图来"，否则构图被锁死（同人双胞胎/相机不动）。
- 什么时候用 / 常见坑：适合音乐人/翻唱区/想批量做 MV 的人；Higgsfield 按 credits 计费，量产前先拿试作版（ComfyUI 本地 720p）验流程；日文原帖，核心已提炼。

**适用场景**：音乐人、翻唱/混剪区 UP 主、想接 MV 商单的人。

**怎么用它搞钱**：AI MV 代做 / 音乐人宣传片商单。

**来源**：[@aisongman](https://x.com/aisongman/status/2112789402053484904)（附 1 分钟成片）· 2026-10-21

### @ai_goge（Daniel.S）：Claude 被封后，我开始用 Cursor 做视频——Opus 5.5 + Remotion 12 官方 Skill 全流程

**核心提炼**
- 解决什么问题：Claude 账号被封后，用 Cursor 跑 Opus 5.5 + Remotion 做动画——从第一条提示词到导出 MP4 的完整实操记录，10 分钟跑通第一条。
- 开工前三条铁律：默认只预览不渲染（不明确说"渲染/导出/给我 MP4"，Opus 只开 Studio 预览）；配音默认走 ElevenLabs（要 API Key）；字幕用本机 GPU 跑 Whisper（免费，Mac 第一次要实测）。分工一句话：你出判断、Opus 写代码、Studio 预览、Remotion 出片。
- 10 分钟跑通：Cursor Agent 模式（不是 Ask）打开 ~/remotion-videos→读 remotion-best-practices 总路由→remotion-create→npx remotion studio 浏览器预览→src/ 写组件→Root.tsx 注册→说"渲染成 MP4"导出（也可点 Studio 右上角 Render 按钮）。
- 12 官方 Skill 地图：总路由 best-practices；create（新建，npx create-video --blank）；markup（80+ 特效，动画只能 useCurrentFrame()+interpolate() 驱动）；interactivity（Studio 直接拖改自动写回代码，省 token）；captions（本机 Whisper 逐词高亮）；maps / multimedia / docs / studio / render / saas（批量：Player/Lambda/自建渲染）/ upgrade。
- 路线规划：15 秒竖版金句卡跑通→沉淀成模板→加声音→批量（一份 JSON/表格放 10 条观点，脚本批量渲染 10 条视频）。
- 什么时候用 / 常见坑：适合想用 Cursor/Claude Code + Remotion 做代码化视频的人；技能装在 ~/.agents/skills/（Cursor）与 ~/.claude/skills/，版本 4.0.536 需与项目一致；小改 Studio 里拖、大改再找 Opus（省 token）；Agent 必须在正确文件夹里开，否则它会去别处建项目。

**适用场景**：想搭 Remotion 代码视频管线、不熟悉 React 的创作者。

**怎么用它搞钱**：金句卡/知识动画批量代做 / Remotion 管线搭建服务。

**来源**：[@ai_goge](https://x.com/ai_goge/status/2112731798811894180) · 文章：[Claude 被封后，我开始用 Cursor 做视频](https://x.com/i/article/2112717418980392960) · 2026-10-21

### @Decoded08：4 个 Prompt 把品牌 brief 变成 30 秒动态排印广告

**核心提炼**
- 解决什么问题：传统动效=时间线+模板库+一下午关键帧——4 个 prompt 把虚构品牌 POPSY 从文字 brief 做到 30 秒 kinetic-typography promo：浏览器里播放、可换字给任何客户、可录成视频文件。
- 核心用法（4 步）：1) Claude 写一页 brief（品牌/受众/6 个定时场景+每场景确切文案+每词动效+配色+字体），存 brief.md 当 single source of truth（每节拍 1–4 个词，文案多了再好的代码也救不了）；2) Claude Code 读 brief.md 写 index.html/style.css/script.js，打开即播（central timeline+固定场景时间，scrub/loop/record 才可靠）；3) 加控制与录制：播放/暂停/scrubber、16:9/9:16/1:1 切换、live text editor 换字、Record 导出 .webm（每种画幅都测一遍，竖屏会挤）；4) premium polish：overshoot easing、motion blur、film grain、beat-locked timing（polish 最后加，先盖 bug 只会更显眼）。
- 三个坑：屏上词太多、散乱 setTimeout（用 central timeline）、录制前不查画幅。
- 什么时候用 / 常见坑：适合小品牌 launch promo、Gumroad 卖可换字模板、月度剪辑包、YouTube 片头；工具只有 Claude（免费版够写 brief）+Claude Code+浏览器+空文件夹，无视频编辑器无模板无插件；英文原帖，附 YouTube 完整教程。

**适用场景**：接小品牌广告/宣传片的人、想卖可复用视频模板的人。

**怎么用它搞钱**：小品牌 launch promo 代做 / Gumroad 卖可换字模板 / 月度剪辑包订阅。

**来源**：[@Decoded08](https://x.com/Decoded08/status/2112781923500302726)（附 YouTube 完整教程）· 2026-10-21

### @GoSailGlobal（Jason Zhu）：16 个做视频 Skill 同题实测——只推 3 个

**核心提炼**
- 解决什么问题：16 个做视频的 skill 做同一条 15 秒宣传片，全部过关——但差别巨大：什么都不装的 Claude Code 也过关（4.4 分钟），说明 skill 的价值不在"能不能做"，而在时间/声音/长相。
- 实测数据（同题 15 秒片用时）：explainroo 2.0 分钟（最快）、不装 skill 4.4、Remotion 官方 4.5、onetake 8.5、motion-video-kit 21.8、hyperframes 23.5（最慢）；16 个里 9 个自己做了声音，6 个和不装的长得很像；只推 3 个。
- 什么时候用 / 常见坑：选型参考——先看这份实测再决定装哪个 skill，别盲目全装；16 条成片在 agentskillshub.top 可直接播放对比；GitHub 合集 zhuyansen/awesome-claude-video-skills（772★，2026-10-20 更新）；附 YouTube 高清版《Claude Code 做视频要装哪个 Skill？》；注：此 Jason Zhu 与 @zhu185178（Feicai）不是同一人。

**适用场景**：要在众多视频 skill 里选型的人、想评估 skill 真实水平的人。

**怎么用它搞钱**：按这份实测给客户搭管线做代建 / skill 选型咨询。

**来源**：[@GoSailGlobal](https://x.com/GoSailGlobal/status/2112801857144029440)（附 3:06 演示视频）· 合集：[zhuyansen/awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills)（⭐772 · 更新于 2026-10-20）· 2026-10-21

### @S1MP23503787（Visionary）：本地模型 AI 模特生成全流程——12GB 显存跑通图+视频

**核心提炼**
- 解决什么问题：RTX 5070（12GB 显存）本地跑通"想法→提示词→照片→换头/换发型/换姿势/换机位→360°环绕和舞蹈视频"全流程——新手向的 ComfyUI 本地化生产工作流，Codex 当搭建助手。
- 模型配置（INT8 量化+分阶段加载，12GB 显存的关键）：生图/编辑 Qwen-Image 2.1（INT8 ConvRot）+文本编码 Qwen3-VL 8B；换头 BFS Head V1.1；换姿势 Fisher Pose+VNCCS PoseStudio；换机位 QMA Camera Angles LoRA；视频 MiniMax H3 FL2VA Pruned（INT8）+360 Orbit LoRA；脸部修复 Director FaceRefine；Codex 查配置/读写工作流/排错。
- 完整流程：普通生图（先立住人物画面）→换头（BFS，跨服装场景保连续性）→换发型（文字直改免蒙版）→换姿势（骨架预设）→换机位（QMA LoRA 出多镜头）→360°环绕（H3+Orbit LoRA：首尾同一张图、768×768、73 帧、28 步）/跳舞（H3 图生视频：4 秒、448×448、24fps、8 步加速）→FaceRefine 自动检测跟踪重绘人脸→导出。
- 安装验证顺序：普通生图→单项编辑→H3 短视频→环绕→舞蹈→FaceRefine，每过一关保存可用版本；权重 huggingface.co/Comfy-Org/Qwen-Image-2.1、Comfy-Org/MiniMax-H3。
- 什么时候用 / 常见坑：适合想本地化部署 AI 写真/短视频产能的人（数据私有、不烧云 credits）；12GB 能跑≠全模型常驻，靠量化+分阶段加载+内存卸载；环绕视频属生成式结果，产品级几何展示仍需逐帧检查；脸部修复保留前后双版本对比挑。

**适用场景**：AI 写真/电商模特从业者、想本地化视频产能的工作室。

**怎么用它搞钱**：AI 模特写真代做 / 电商服装换模特服务 / 本地化部署咨询。

**来源**：[@S1MP23503787](https://x.com/S1MP23503787/status/2112798918094516435) · 文章：[利用本地模型，最大程度开发AI模特生成功能（新手分享版）](https://x.com/i/article/2112798521133068289) · 2026-10-21

### @awe0_io：Y2A-Auto——YouTube 扒片→AI 翻译→B 站/AcFun 一键发布的无人搬运流水线

**核心提炼**
- 解决什么问题：搬运号的人工链路（下载→翻译→压字幕→上传）太费人；这条无人流水线从 YouTube 扒视频、AI 翻译加字幕、内容审核、智能监控，到一键发布 B 站和 AcFun，全程不用动手。
- 核心用法（4 步）：1) 部署开源项目 fqscfqj/Y2A-Auto（GPL-3.0，3936★，2026-10-20 仍在更新）；2) 配好源站与目标站账号；3) 设定抓取规则、翻译与字幕参数；4) 开启智能监控，流水线自动跑。
- 什么时候用 / 常见坑：做搬运矩阵、跨平台分发时用；搬运有版权与平台合规风险，先确认内容授权再放大；监控告警要配好，别让违规内容自动发出。

**适用场景**：搬运号矩阵、跨平台内容分发、想零人工跑账号的人。

**怎么用它搞钱**：搬运矩阵号 / 跨平台分发代运营。

**来源**：[@awe0_io](https://x.com/awe0_io/status/2112872752059420714) · 项目：[fqscfqj/Y2A-Auto](https://github.com/fqscfqj/Y2A-Auto)（⭐3936 · GPL-3.0 · 更新于 2026-10-20）· 2026-10-21

### @linda6248130564（财经老王）：17 岁少年的 AI 短视频矩阵流水线

**核心提炼**
- 解决什么问题：一个人怎么做 12 个 YouTube Shorts 频道——整套 AI 流水线：Claude 产出选题 → ElevenLabs 生成配音 → CapCut 自动成片 → Python 脚本定时发布；不用拍摄、不露脸、不用手动剪辑。
- 核心用法（4 步）：1) 每条赛道独立运营、频道分开；2) Claude 批量产选题脚本；3) ElevenLabs 配音 + CapCut 模板化成片；4) Python 定时发布，全流程大部分自动。
- 什么时候用 / 常见坑：自述日工作 3 小时、日产 24 条、单频道月入 8k–1.5W 美元、月入 10W+ 美元——为发帖人自述收益，未经第三方核实，按经验打折看；矩阵号起量期适用，单账号精耕不适用。

**适用场景**：想做 Shorts/短视频矩阵、批量起号的人。

**怎么用它搞钱**：Shorts 矩阵号 / 批量起号代运营。

**来源**：[@linda6248130564](https://x.com/linda6248130564/status/2112819290416329041) · 2026-10-21

### @zdt0403（PigcW）：Remotion 批量做视频实测——把片子做成模板才是值钱用法

**核心提炼**
- 解决什么问题：代码做视频（Remotion）怎么从"做一条"变成"出一条产线"——核心判断：值钱的用法是把片子做成模板，从第二条起每条成本只剩一份 data.json 加几秒渲染；翻车基本出在数据（数字太长、没来源、标题太长），很少出在动画本身。
- 核心用法（7 步）：1) 建项目；2) Agent 先做一条满意样片（先写 story.md：一个观点、一个主数字、三拍）；3) 冻结成模板（文字数字全从 props 读、时长/延迟/缓动集中到 timing.ts、画幅由 props.format 决定）；4) 定数据规范（每个数字必须带 source，数字/标签/单位分开写）；5) 批量脚本（bundle 一次，循环：预检→选 composition→渲关键帧→渲成片）；6) 验收脚本（静帧扫安全区、ffprobe + blackdetect + freezedetect 查黑段冻帧，不过的进 failed 文件夹）；7) cron 定时跑，人只看拼图抽检。
- 什么时候用 / 常见坑：实测数据——JSON 进→12.5 秒竖版、Node API 渲染 6.9 秒、冷打包 10.1 秒/有缓存 1.4–2.4 秒；每周一期×52 期×3 画幅=156 个文件，全年渲染约 25 分钟；许可——个人/非营利/≤3 人营利公司免费（含商用），超 3 人公司须买授权；发布不建议全自动，数据类视频错一个数比晚发一天麻烦；成本账（转述未核实）：3 分钟科普片全代码成本不到 0.5 美元。与 @ai_goge 的 Claude+Cursor+Remotion 帖为不同作者、不同角度（实测+验收脚本+成本账），属增量干货。

**适用场景**：资讯号、数据号、知识号的周更栏目；会 React 的小团队。

**怎么用它搞钱**：卖"每周能自己出片的模板"（作者原话：别卖"帮你做一条 AI 视频"）/ 数据栏目代运营。

**来源**：[@zdt0403](https://x.com/zdt0403/status/2112889851934892120) · 文章：[Remotion 批量做视频实测长文](https://x.com/i/article/2112889829860188160) · 2026-10-21

### @SPCXBTC（米奇 Mickey）：《AI 短剧交战手册》——成本、工具、团队、分账公式一篇拆完

**核心提炼**
- 解决什么问题：AI 短剧到底赚不赚钱、怎么干——一篇整合多家媒体报道与从业者案例的合成长文，拆了成本、工具、团队配置、流量换收入公式和死法。
- 核心用法（7 要点）：1) 成本账：AI 漫剧约 800–1200 元/分钟，AI 仿真人剧整部约 6–10 万元，同体量真人剧 50 万元以上（约为真人 1/5 到 1/10）；2) 工具链：视频生成即梦 Seedance 2.0/2.5、Vidu、可灵 3.0，全流程 Agent/平台（小云雀短剧 Agent、巨日禄、昆仑天工、可梦 AI），Suno 配乐、豆包/ChatGPT 写分镜提示词；3) 团队：真人剧组约 40 人→AI 剧组 10 人以内甚至两三人；4) 收入公式：利润 ≈（有效时长 × 单价 × 系数）−（算力 × 抽卡倍数 ＋ 人力 ＋ IP ＋ 投流），分账按时长不按播放量；5) 实操：选现成 IP 改编→先做 3–5 集样片测数据→单集 1.5–3 分钟→钩子前置→锁角色一致性→先备案→做系列不做单部；6) 风险：下架（未备案/题材合规）、单价下滑、卖课晒收益陷阱；7) 结论：这是低成本试错公式不是暴富公式，真正赚钱的是能连载、合规、做得快的 1%。
- 什么时候用 / 常见坑：合成长文非一手实测，部分数字为单一来源或作者推算（如单价、ROI），看趋势不看精确值；2026 年 4 月 1 日起 AIGC 微短剧先备案后上线，仿真人还需人物授权和三视图。

**适用场景**：想入场 AI 短剧/漫剧的团队和个人、做选题判断的人。

**怎么用它搞钱**：AI 短剧/漫剧制作接单 / 剧本改编代运营。

**来源**：[@SPCXBTC](https://x.com/SPCXBTC/status/2112886505446236346) · 2026-10-21

### @Justin_lords：AI 电商广告素材自动化管线——竞品拆解到自动拼接

**核心提炼**
- 解决什么问题：电商广告素材要高频产出、人工剪辑跟不上——四步管线：①找 TikTok/Meta 竞品爆款广告，喂给 Gemini 拆解 hook、叙事结构和逐场景视觉提示词；②用 Seedance、Kling 或 OmniFlash 生成视频片段；③UGC 口播钩子用 ElevenLabs 变声做得更真实；④用自定义 FFmpeg 或 Claude MCP Premiere Pro 连接自动拼接，省掉手动剪辑。
- 核心用法（4 步）：按上面四步走，素材生产从"一条条剪"变成"喂竞品→出成片"。
- 什么时候用 / 常见坑：成本账（作者自述）：$500/条 UGC vs 几美分到几美元/条 30 秒 AI 素材，$2–5/天产出多条；帖子结尾带关注引流，方法部分实质成立、营销话术自行过滤；Gemini 拆解质量决定下限，先拿跑通的爆款喂。

**适用场景**：电商卖家、广告投手、代运营团队的素材部门。

**怎么用它搞钱**：电商广告素材代制 / 测品素材包。

**来源**：[@Justin_lords](https://x.com/Justin_lords/status/2112883550697779545) · 2026-10-21

### @zhu185178（Feicai）：Codex Agent 全流程做视频——人只负责选题和脚本

**核心提炼**
- 解决什么问题：Agent 做视频能不能端到端——管线五阶段：找素材→旁白声音克隆→剪辑→视频包装→统一调色，人只负责选题/脚本，其余全部由 Codex 完成；视觉包装已提炼为可重复使用的通用设计。
- 核心用法：模型配置 GPT-6 Astra、推理开 max；同一套视觉包装换主题稳定输出。
- 什么时候用 / 常见坑：成片帖，完整教程作者预告后续更新；与本账号早档"Opus 5.5 广告分镜师"是不同工具链（Codex vs Opus 5.5），互为对照。

**适用场景**：想用 Codex 跑完整视频制作流程的创作者。

**怎么用它搞钱**：知识/科普视频代制 / 栏目化内容代运营。

**来源**：[@zhu185178](https://x.com/zhu185178/status/2112886367566873005) · 2026-10-21

### @zhu185178（Feicai）：Opus 5.5 vs Codex 做视频效率对比——差 3 倍

**核心提炼**
- 解决什么问题：两个 Agent 做视频到底差多少——效率对比数据：Opus 5.5 约 1–2 小时 vs Codex 6 小时+，效率差 3 倍；方法论：主题/脚本→视频 + 通用包装视觉组件，换主题稳定输出。
- 核心用法：科普/知识类选题优先用 Opus 5.5 跑，平台（抖音/小红书/B 站）正在推知识大赏系列，门槛下降是流量窗口。
- 什么时候用 / 常见坑：为 Codex 全流程帖的前传，两帖各有增量；效率数据为作者单次实测，换选题可能浮动。

**适用场景**：Agent 视频选型、知识区账号起号。

**怎么用它搞钱**：知识大赏系列账号 / 测评类内容。

**来源**：[@zhu185178](https://x.com/zhu185178/status/2112867047889924220) · 2026-10-21

### @Steel_web（Sophie_404）：motion designer agent studio——spec.md+assets/+render.py，edit 就是 git diff

**核心提炼**
- 解决什么问题：把 Claude Code 从聊天机器人变成"睡觉时也在渲染的工作室"——技术栈极简：一个文件夹 = spec.md + assets/ + render.py，Claude 写场景、引擎逐帧渲染、ffmpeg 合成音频；没有时间线、没有关键帧，edit 就是 git diff。
- 核心用法（3 要点）：1) 迭代免费："把运镜放慢"不是给外包提需求，而是改一个参数，一夜跑 200 个同镜头变体，成本只是 token；2) 实验量是新的能力天花板；3) 管线不是"AI 做视频"，而是"agent 做那个做视频的东西"。
- 什么时候用 / 常见坑：主帖与"agents make the thing that makes the video"线程（午档已收录）同源，本条为作者自回复链补充的架构与迭代成本论，增量入库；三条 elaboration 下各有 1 条嵌套回复未深挖，现有实质已足。

**适用场景**：动效设计师、想搭个人渲染工作室的创作者。

**怎么用它搞钱**：动效模板/片头代制 / 个人工作室接单。

**来源**：[@Steel_web](https://x.com/Steel_web/status/2112802427330040259)（作者自回复链：技术栈/迭代成本/端到端 dossier）· 2026-10-21

## 收录标准

- 来源：X 博主实战分享（原帖 / 评论区 / 引用链）及 GitHub 高星项目
- 每条格式：核心提炼（解决什么问题 / 核心用法 3–5 步 / 什么时候用与常见坑）+ 适用场景 + 「怎么用它搞钱」+ 来源（Star 数与最近更新时间）
- Star 数与更新时间为 2026-10-21 经 GitHub API 核验；持续收录中
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

- 2026-10-21：晚档搜集（优先队列第 10 天）——X 新增 8 条管线实战帖提炼入库：@awe0_io Y2A-Auto 无人搬运流水线（YouTube 扒片→AI 翻译→B 站/AcFun 一键发布）/ @linda6248130564 17 岁少年 AI 矩阵（Claude 选题→ElevenLabs 配音→CapCut 成片→Python 定时发布）/ @zdt0403 Remotion 批量做视频实测长文（模板化+三道验收+7 步搭自动出片线）/ @SPCXBTC《AI 短剧交战手册》（成本/工具/团队/分账公式/风险一篇拆完）/ @Justin_lords 电商广告素材自动化管线（Gemini 拆解竞品→Seedance/Kling 生成→FFmpeg 自动拼接）/ @zhu185178×2（Codex Agent 全流程做视频 + Opus 5.5 vs Codex 效率对比差 3 倍）/ @Steel_web agent studio 架构自回复链（spec.md+assets/+render.py，edit 就是 git diff，午档线程的增量补充）；fqscfqj/Y2A-Auto 经 API 核验（3936★ · GPL-3.0 · 更新于 2026-10-20）；8 帖正文与时间戳经 fxtwitter API 逐条直读核验；15 个指定账号时间线全部抽查完毕，无遗漏；全程只读、未遇真人验证（@Steel_web 帖子页曾误触回复按钮，已立即关闭未发布）

- 2026-10-21：午档再补录（优先队列第 10 天）——第二份迟到报告（重派任务）送达，确认 14 命中，X 新增 4 条提炼入库：@ai_goge Claude+Cursor+Remotion 12 官方 Skill 全流程（10 分钟跑通/批量路线）/ @Decoded08 4 prompt 动态排印广告管线（brief.md single source of truth）/ @GoSailGlobal 16 个视频 skill 同题实测（只推 3 个，合集 772★）/ @S1MP23503787 本地 ComfyUI AI 模特图+视频全流程（RTX 5070 12GB，Qwen-Image 2.1+MiniMax H3）；@Steel_web 线程确认为 5 帖（已收录 3 帖核心无误）；@CrazyKaomei 火柴人风格 5 仍按宁缺毋滥未收；4 帖正文与时间戳经 fxtwitter API 逐条直读核验

- 2026-10-21：午档补录（优先队列第 10 天）——迟到的浏览器任务报告送达（15 组关键词×Latest+10 账号时间线全量执行），X 新增 8 条管线实战帖提炼入库：@yuanliuwei×4（暗黑数据科普 Skill 6 步流水线 / Vibe 知识大赏保姆级复刻教程 / Grok Bot 0 员工短视频工作室 7 条产线 / 心理科普 Skill 5 步流水线，均 MIT 开源）+ @justloveabit huashu-motion（一句话出 30 秒 4K 宣传片，"指着画面改"，1194★）+ @xiaohu AI 日报视频版 Demo（Claude Code 全流程+模板自动化）+ @lisenhai9999 YouTube Shorts 月入 $1200 四步管线 + @aisongman Claude Code 全自动 MV（2K 唇形同步，232 credits）；@CrazyKaomei 火柴人风格 5 为技能更新帖非管线方法论、按宁缺毋滥未收；8 帖正文与时间戳均经 fxtwitter API 直读核验，6 个仓库 star/更新时间经 API 核验

- 2026-10-21：午档搜集（优先队列第 10 天）——X 新增 2 条管线实战帖提炼入库（@Steel_web Claude Code 代码驱动动效管线：spec.md+render.py+ffmpeg，"edit 就是 git diff" / @drahcir_rahl Hermes 端到端视频工具链：OpenScreen 采集+HyperFrames 制作+无头后期装成一个 skill，仓库 rahlquist/hermes-video-toolchain 经 API 核验真实）；浏览器任务报告链路故障（任务执行完毕但报告未送达），2 条为任务执行中实际打开核验的帖子经 fxtwitter API 直读补全

- 2026-10-21：早档搜集（优先队列第 10 天）——X 新增 6 条管线实战帖提炼入库（@techniqco n8n 企业级 Shorts 管线 / @Chenfacai0 Toonflow 短剧流水线 / @xoyif63862452 7 套 Skills 选型地图 / @qinghaiwu9527 WorkBuddy 漫剧智能体团队 / @justloveabit HyperFrames 实操 / @zhu185178 Opus 5.5 广告分镜师）+ GitHub 新增 3 个项目（AutoVio / Video Generation Workflow Skill / Remotion Idea to Video），6 个老条目 star 与更新时间刷新

- 2026-10-12：6 个项目条目按铁律升级（表格→小节：补核心用法 / 常见坑 / 适用场景 / 来源，Star 数与更新时间重验）
- 2026-10-11：首版，6 个项目，持续收录中
