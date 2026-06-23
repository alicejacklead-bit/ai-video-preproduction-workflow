# AI 视频生成前期工作流

这个仓库现在同时是一个可安装的 Codex skill。仓库根目录包含 `SKILL.md`、`agents/openai.yaml` 和 `references/`，可以作为独立 skill 使用。

## 安装

在 Codex 里可按 GitHub 仓库方式安装这个 skill：

- Repository: `alicejacklead-bit/ai-video-preproduction-workflow`
- Skill name: `ai-video-preproduction-workflow`

这是一个用于 AI 视频创作的前期控制工作流仓库，核心思路是先完成导演层定义，再进入生成阶段。项目通过 `创意选题 -> Plan Demo -> 人物形象图 -> 场景图 -> 导演机位图 -> 分镜图 -> 封装图 -> 视频提示词` 这一套资产链，尽量稳定角色一致性、空间连续性与镜头逻辑。

## 项目目标

这套方法面向多种视频类型，目标是把“靠一条长提示词碰运气”改成“先搭建可控资产，再稳定生成”的流程：

- 在生成前固定角色外观与行为特征
- 在生成前固定空间布局与运动路线
- 通过导演机位图控制正反打、视线和笑点揭晓
- 用封装图和提示词统一交付给视频模型

## 交付内容

- [Methodology Document](andy-ai-video-generation-workflow.md)
- [导演方案](docs/plan-demo.md)
- [成片封装图](assets/package-showcase.svg)
- [人物形象图](assets/character-board.svg)
- [场景图](assets/scene-layout.svg)
- [导演机位图](assets/director-camera-map.svg)
- [分镜图](assets/storyboard-showcase.svg)
- [成片提示词](prompts/showcase-video-prompt.txt)
- [发布文案](copy/release-copy.md)

## 目录结构

- `assets/`：封装图、分镜图、人物图、场景图与机位图等视觉资产
- `prompts/`：视频模型提示词
- `docs/`：导演方案与项目说明
- `copy/`：对外发布文案
- `projects/`：英文版项目拆解与沉淀
- `single-video-projects/`：single-project breakdowns and delivery records

## 适用类型

- 剧情短片
- 情景喜剧
- 动物剧场
- 产品演示视频
- 品牌创意广告
- UGC 带货视频
- workflow showcase content

## 方法概览

1. 先定义角色形象，锁定服装、表情与动作习惯。
2. 再定义场景布局，锁定家具关系、出入口与移动路径。
3. 用导演机位图固定摄影机位置与镜头职责。
4. 将关键镜头映射到分镜图，明确每个镜头的叙事任务。
5. 最后把上述信息汇总为封装图和提示词，交给视频模型生成。

## 当前示例项目

仓库当前附带的主示例，是一条 15 秒欧美公寓情景喜剧短片，用来演示这套流程如何控制多人对话、固定空间关系和完成笑点反转。

- 类型：情景喜剧短片
- 时长：15 秒
- 画幅：16:9
- 角色：两个人类角色与一只橘猫
- 用途：展示工作流，而不是限定工作流只能用于喜剧内容

## 适用场景

- AI 视频前期策划与导演拆解
- 多镜头对话类视频生成
- 需要控制空间连续性的内容创作
- 可复用的视频提示词封装流程
