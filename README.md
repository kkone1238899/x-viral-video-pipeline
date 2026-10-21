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

- 2026-10-21：早档搜集（优先队列第 10 天）——X 新增 6 条管线实战帖提炼入库（@techniqco n8n 企业级 Shorts 管线 / @Chenfacai0 Toonflow 短剧流水线 / @xoyif63862452 7 套 Skills 选型地图 / @qinghaiwu9527 WorkBuddy 漫剧智能体团队 / @justloveabit HyperFrames 实操 / @zhu185178 Opus 5.5 广告分镜师）+ GitHub 新增 3 个项目（AutoVio / Video Generation Workflow Skill / Remotion Idea to Video），6 个老条目 star 与更新时间刷新

- 2026-10-12：6 个项目条目按铁律升级（表格→小节：补核心用法 / 常见坑 / 适用场景 / 来源，Star 数与更新时间重验）
- 2026-10-11：首版，6 个项目，持续收录中
