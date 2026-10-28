<!-- ✨ 顶部 banner（柔和薄荷绿 + 米色插画风，本地 SVG，零依赖） -->
<div align="center"><img src="assets/banner.svg" width="100%" alt="Shanxia Wen banner" /></div>

## 👋 Hi there

你好，我是 **温珊霞（Shanxia Wen）** —— 一名想把「AI 能力」翻译成「能上线的业务功能」的全栈开发者。2027 届，计算机科学与技术专业，base 广州。

我关注 AI 的最新进展，但更在意它能不能落地：**用 AI Agent 把采购系统里那些要反复点选、反复核对的流程，压缩成一句话就能完成**；也用 Spring Boot 把交易、库存、审批这些最容易出事的环节守住。

做过的两个完整项目，一个在把电商的「钱和货」对齐，一个在把采购的「单据和账」对齐。它们教会我同一件事：**功能能跑起来只是及格线，数据不出错才是真正的交付。**

> 追求前沿很重要，但我更愿意先把它做成可交付、可维护、可复盘的东西。
>
> *Following the AI frontier — and turning it into shippable, reproducible engineering.*

---

## 🔧 我正在做什么

| 方向 | 实施内容 |
| :--- | :--- |
| 🤖 **AI Agent 工程化** | 用 **Spring Boot + LangChain4j + 通义千问** 做采购智能体：`@Tool` 注册报表、订单、库存、结算、收货五类业务工具，大模型自主解析口语需求并跨工具编排；并用**数据校正 + 逐字段校验 + 后端确定性生成**三道防线管住幻觉 |
| 🌐 **全栈业务开发** | **Spring Boot + Vue2 / React + TypeScript** 独立完成两个系统：交易与库存一致性、Sa-Token + RBAC 权限、SSE 流式推送、ECharts 运营看板、支付宝异步回调验签 |
| 🎨 **AI 生成内容工程化** | 实习期间用 **ComfyUI 搭节点工作流**、调高清放大参数、筛 LORA 资源，建立标准化批量出图流程，解决 AI 出图"五官失真、画风不统一"的老问题 |
| 🧱 **基础与成长** | 专业成绩前 15%，拿过**优秀学生奖学金**，通过**软考中级 · 软件设计师**；持续补数据结构、算法与操作系统等底层基础 |

---

## 🎓 教育 & 技能

**广州理工学院** · 计算机科学与技术（本科）　`2023 — 2027`

| 类别 | 内容 |
| :--- | :--- |
| 📖 **主修课程** | Java、Python、数据结构与算法、计算机网络、操作系统、MySQL、软件工程、人工智能 |
| 🏅 **学业表现** | 专业成绩位列**前 15%**，获**优秀学生奖学金** |
| 📜 **证书** | 国家软考中级 · **软件设计师** |
| ⚙️ **技术框架** | Spring Boot、Vue、HTML、uni-app、MyBatis(-Plus)、Redis、Docker、Git、GoLand、鸿蒙开发工具 |
| 💻 **开发环境** | Java、VS Code、IntelliJ IDEA、GitHub；熟练使用 Office（Excel / PowerPoint） |
| 🤖 **AI 工具** | Codex、WorkBuddy、Claude、Trae、Coze、ChatGPT、Gemini、DeepSeek、通义千问、飞书 |

---

## 💼 实习经历

**广州灵创互联网科技有限公司** · AI 图像设计师　`2025.10 — 2026.01`

- 独立负责 **AI 图像生成**业务，主导 **ComfyUI 节点工作流**搭建与高清放大参数调优，解决**五官失真、画风不统一**两大痛点
- 高效筛选优质 **LORA 资源**，建立**标准化批量出图流程**，显著提升团队整体交付效率

> 抬头写的是"设计师"，做的其实是生成式 AI 的工程化。这段经历让我第一次意识到：模型效果不是调 prompt 调出来的，而是被**工作流和参数**约束出来的 —— 这个认知后来直接搬进了我的 AI Agent 项目。

---

## 📂 代表项目

### 🛒 助农电商平台 · 全栈开发者　`2025.07 — 2025.08`

`Spring Boot` `MyBatis-Plus` `MySQL` `Redis` `Sa-Token` `Vue2` `Element UI` `ECharts` `支付宝支付` `Druid`

- **交易与库存一致性**：下单实时校验并扣减库存，不足则拦截，扣减后联动缺货标记与下架；**支付宝沙箱异步回调 RSA 验签**扭转订单状态，Redis 缓存承担下单压力并支持合并支付，打通退款链路、规避超卖
- **认证鉴权与权限**：基于 **Sa-Token** 实现登录鉴权、密码加盐、账号封禁与同端互踢；**RBAC** 角色模型，后端全局异常统一收敛越权与封禁，前端路由按角色鉴权
- **采购与售后闭环**：供应商、采购单与收货入库回填库存，打通"采购—销售"链路；退货申请可配置原因，**售后全程可追溯**
- **运营看板与营销**：ECharts 聚合商品 / 订单 / 退货多维指标，按时间筛选趋势与占比；落地 **VIP 会员与轮播营销位**
- **工程化**：统一响应体规范；集成邮件模板异步发送、**敏感词 DFA 过滤**、**Druid** 连接池

### 🤖 基于 Spring Boot 与 AI Agent 的采购管理系统 · 全栈开发者　`2026.08 — 2026.09`

`Spring Boot` `MyBatis-Plus` `MySQL` `Redis` `LangChain4j` `SSE` `React` `TypeScript` `Ant Design 5`

- **AI 对话 Agent 模块**：基于 **LangChain4j 接入通义千问**，`@Tool` 注册报表、订单、结算、收货等五类业务工具，大模型自主解析口语需求并跨工具编排；自动解析时间范围并做**用户数据隔离**，异常时自动降级关键词路由；针对幻觉设计**后端数据校正 + 逐字段替换为真实业务数据 + 确定性生成**，单据变更后对话结果实时联动
- **智能预警中心**：**策略模式**落地 7 类可配置预警规则（订单逾期、审批超时、低库存、发票异常等），支持阈值配置与告警自动升级；重构去重机制，以数据状态为准、**Redis 负责并发防重**；依托 **SSE 流式推送**支持心跳保活、断线重连与消息补偿，处置全程留痕
- **用友式三单匹配**：把整单比对改造为**行级数量多对多匹配**，适配一单多收、一票多单；支持多维度比例 + 绝对金额容差，实现暂估回冲；超容差单据自动冻结，付款前强校验匹配状态
- **采购链路稳定性治理**：单据状态机流转、收货**超收硬拦截**、撤销收货自动回冲；库存扣减乐观锁防超卖，金额由后端明细重算；两级审批用 **Redis 锁 + DB 乐观锁**防并发；封装全局异常、数据权限切面与审计字段自动注入

---

## 🧿 联系我

2027 届在校生，求职方向 **IT 类 / Java 全栈开发**，期望城市 **广州**。欢迎校招与实习机会，也欢迎纯粹的技术交流。

📮 邮箱：**3163350557@qq.com**

---

<div align="center">

### 你好，我是 温珊霞

<p>
  <a href="https://github.com/NanaWanWen"><img src="https://img.shields.io/badge/GitHub-NanaWanWen-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="mailto:3163350557@qq.com"><img src="https://img.shields.io/badge/Email-3163350557@qq.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/广州-2027届求职中-6DB33F?style=for-the-badge" />
</p>

<img src="https://ghchart.rshah.org/8ac48a/NanaWanWen" alt="NanaWanWen contribution chart" width="92%" />

</div>




