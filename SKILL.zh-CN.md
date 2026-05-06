---
name: ai-infra-investing
description: 当用户要分析 AI 相关股票、ETF 或组合，并希望按 AI 基建层级、组合分桶、加减仓触发条件来判断时使用。适用于 AI 平台龙头、芯片、内存、代工封装、GPU 云运营商、AI 支付结算、组合构建、仓位优先级、核心仓与高 beta 交易仓区分等场景。
---

# AI 基建投资

这个 Skill 不是用来找短线买点的，而是用来把 AI 投资问题拆成可管理的结构。

它主要解决 4 类问题：
- AI 主线里，这家公司属于哪一层
- 这只股票应该放在组合的哪个桶里
- 应不应该买，应该买多大
- 什么情况下加仓，什么情况下减仓

它不适合：
- 日内交易
- 精确价格预测
- 期权结构设计
- 完整估值模型

## 适用场景

当用户问下面这类问题时，优先使用这个 Skill：

- “这只股票在 AI 叙事里属于哪一层？”
- “这只股票该算核心仓还是主题仓？”
- “AI 组合应该怎么搭？”
- “GPU、CPU、内存、封装、光模块、运营商怎么分层看？”
- “这只股票应该先买还是先观察？”
- “哪些是底仓，哪些只能做弹性仓？”
- “什么时候应该加仓或减仓？”
- “高 beta 的 AI 股票该怎么控制仓位？”

如果问题重点是：
- 股票性格
- 波动体验
- 能不能拿得住
- 历史上涨/回撤像什么波浪

那就把 `wave-investing` 当成补充视角一起用。

## 工作流

按这个顺序来：

1. 先判断这只股票属于 AI 基建哪一层。  
读取 [references/ai-stack-layers.md](references/ai-stack-layers.md)

2. 再判断它属于组合里的哪个桶。  
读取 [references/portfolio-buckets.md](references/portfolio-buckets.md)

3. 再决定它是否值得进组合。  
有些股票只适合观察，或者只适合交易，不应该硬塞进核心持仓。

4. 把“公司好不好”和“仓位该不该大”分开。  
好公司也可能只值得小仓。

5. 明确写出加仓和减仓触发条件。  
读取 [references/triggers.md](references/triggers.md)

6. 如果它属于高 beta 运营商、主题放大器、矿转 AI、GPU 云租赁这类名字，要额外谨慎。  
读取 [references/high-beta-rules.md](references/high-beta-rules.md)

7. 如果用户同时持有长期主组合、弹性交易仓、象征性叙事参与仓，要强制分开讨论。  
读取 [references/portfolio-structure.md](references/portfolio-structure.md)

## 核心原则

- 区分 `AI 核心暴露` 和 `杠杆化 AI 暴露`
- 区分 `好公司` 和 `现在适不适合重仓`
- 区分 `叙事相关` 和 `组合必需`
- 不要让高 beta 股票伪装成核心仓
- 仓位大小是独立决策，不是股票排序的自然延伸
- 组合要分层，不要把所有 AI 票混成一团

## 推荐输出格式

默认按这个结构输出：

1. `一句话角色`
这只股票在 AI 叙事里扮演什么角色，在组合里扮演什么角色？

2. `AI 层级`
它属于哪一层？

3. `组合分桶`
核心仓 / 卫星仓 / 主题仓 / 防守仓 / 观察仓 / 纯交易高 beta

4. `为什么重要`
这一层在当前 AI 主叙事里为什么重要？

5. `核心风险`
哪一个风险最可能破坏这条逻辑？

6. `加仓触发`
什么出现后更值得加？

7. `减仓触发`
什么出现后更该减？

8. `权重大致建议`
如果进组合，大概适合多大仓位？

## 标准分桶用词

尽量固定使用这些标签：
- `核心仓`
- `卫星仓`
- `主题仓`
- `防守仓`
- `观察仓`
- `纯交易高 beta`

## 约束

- 如果多个名字本质上表达的是同一层风险，必须明确说它们在重复暴露。
- GPU 云运营商、AI 数据中心运营商、矿转 AI、租赁型 AI 基建票，默认按高 beta 运营商处理。
- 如果用户的 thesis 明确包含 Agent 支付、稳定币结算、可编程支付网络，可以把 AI 支付结算层视为 AI 基建的邻接层。
- 如果用户已经明确把一只票定义成交易仓，除非事实明显冲突，否则要尊重这个定义。
- 多股票比较时，至少给出两种排序：
  - `业务质量 / 持久性`
  - `组合优先级`

## 参考文件

- AI 基建层级：[references/ai-stack-layers.md](references/ai-stack-layers.md)
- 组合分桶：[references/portfolio-buckets.md](references/portfolio-buckets.md)
- 加减仓触发：[references/triggers.md](references/triggers.md)
- 高 beta 规则：[references/high-beta-rules.md](references/high-beta-rules.md)
- 组合结构卡片：[references/portfolio-structure.md](references/portfolio-structure.md)
