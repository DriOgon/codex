# 5个热门skills

> 统计口径：基于 `https://skills.sh/hot` 实时热榜抓取（时间：2026-03-06）。
> 热度字段参考：`installs`（累计安装）与 `change`（近期增量变化）。

## 1) sleek-design-mobile-apps
- 来源仓库：`sleekdotdesign/agent-skills`
- 当前热度：`installs=565`，`change=559`
- 用途：帮助 AI 代理按移动端设计规范产出更一致的 UI/交互方案，适合 App 页面草图、组件规范、设计决策说明。
- 使用方法：
  1. 安装：`npx skills add https://github.com/sleekdotdesign/agent-skills --skill sleek-design-mobile-apps`
  2. 在任务中直接调用：例如“请按 iOS/Android 设计规范，给出登录页布局和组件参数建议”。
  3. 让代理输出可执行结果：页面结构、组件尺寸、间距/字体规则、交互状态说明。

## 2) videoagent-image-studio
- 来源仓库：`pexoai/pexo-skills`
- 当前热度：`installs=58`，`change=58`
- 用途：围绕图片生成与素材处理工作流，适合视频封面、分镜参考图、营销图片草稿生成。
- 使用方法：
  1. 安装：`npx skills add https://github.com/pexoai/pexo-skills --skill videoagent-image-studio`
  2. 提供清晰输入：风格、构图、尺寸、目标平台（如短视频封面/海报）。
  3. 让代理输出“多版本候选 + 提示词迭代建议”，便于快速筛选。

## 3) video-production
- 来源仓库：`supercent-io/skills-template`
- 当前热度：`installs=54`，`change=54`
- 用途：用于视频制作流程化工作，包括脚本拆分、镜头节奏建议、制作清单整理。
- 使用方法：
  1. 安装：`npx skills add https://github.com/supercent-io/skills-template --skill video-production`
  2. 输入你的目标：受众、视频时长、平台（抖音/YouTube/小红书等）。
  3. 让代理输出：分镜表、口播稿、素材清单、发布时间建议。

## 4) react-best-practices
- 来源仓库：`supercent-io/skills-template`
- 当前热度：`installs=53`，`change=53`
- 用途：用于 React 项目的结构优化与代码质量提升，覆盖组件拆分、状态管理、性能与可维护性建议。
- 使用方法：
  1. 安装：`npx skills add https://github.com/supercent-io/skills-template --skill react-best-practices`
  2. 把目标代码或目录交给代理，明确你关心的问题（性能、可读性、重复逻辑等）。
  3. 要求输出“问题清单 + 重构方案 + 风险点 + 回归测试建议”。

## 5) presentation-builder
- 来源仓库：`supercent-io/skills-template`
- 当前热度：`installs=53`，`change=53`
- 用途：快速生成演示文稿内容框架，适合路演、周报、方案汇报、项目复盘。
- 使用方法：
  1. 安装：`npx skills add https://github.com/supercent-io/skills-template --skill presentation-builder`
  2. 给出主题、受众、时长和你希望的结构（背景-问题-方案-结果）。
  3. 让代理输出逐页大纲、每页要点、演讲备注和视觉建议。

---

## 通用安装与调用模板
- 安装模板：`npx skills add https://github.com/<owner>/<repo> --skill <skill-id>`
- 调用建议：在任务里明确 `目标 + 输入约束 + 输出格式`，效果会明显更稳定。
