# CodeSprintMT 2026 Open Category 重点梳理

来源文件：`CodeSprintMT-2026-Open-Category-Competition-Prep-Guide.pdf`

说明：这份 PDF 是 2026 Open Category 的 Preparation Booklet，不是最终完整 Task Booklet。正式题目中的部分细节在评分表里被隐藏为 `...` 或 `Something related to ...**`，PDF 明确说明这些内容会在正式任务书中揭晓。下面按已公开文本完整梳理重点，并把基于资源列表和评分项的方向性判断单独标注为“推断”。

## 1. 文档结构

- 封面：Preparation Booklet，Open Category 2026。
- 目录：
  - Technical Overview
  - Preparation Resources
  - AI-Assisted Coding
  - Judgement Criteria
  - Submission Criteria
  - Rules and Regulations
  - Terms and Conditions
- 欢迎页：参赛者将综合使用 coding、infrastructure、UI/UX design 能力来创建一个 app。

## 2. 技术总览

- 比赛期间需要设计并构建一个 app。
- 评审组已经在一个工作日内做出了 reference implementation，用来证明题目可以在限定时间内完成。
- 比赛当天会提供 reference implementation 的演示。
- 平台不限：
  - Windows
  - macOS
  - Linux
  - Android
  - iOS
  - Web
- 官方推荐 Web 平台，因为可用平台范围更广，但是否使用 Web 不影响分数。
- 开发语言不限，可以使用任何熟悉的编程语言。
- 方案必须能在评委电脑上运行。
- 必须提交：
  - binary / executable solution
  - source code

## 3. 准备资源与技术暗示

PDF 明确说这些资源用于帮助准备任务，并且可以使用任何熟悉的技术。资源列表本身强烈暗示正式题会涉及支付、捐赠、交易、后台管理、实时数据、权限、多币种、导出和对账。

### 3.1 Mastercard Sandbox

- 创建 Mastercard Sandbox 账号：
  - https://developer.mastercard.com/donations/documentation/quick-start-guide/#generate-credentials-and-create-a-sandbox-project
- Mastercard Donate：
  - https://developer.mastercard.com/product/mastercard-donate/
- Donate API 文档：
  - https://developer.mastercard.com/donations/documentation
- Donate API API Reference：
  - https://developer.mastercard.com/donations/documentation/api-reference/
- Donate API API Basics：
  - https://developer.mastercard.com/donations/documentation/api-basics/
- Mastercard Postman workspace，用于先调用 API 再写代码：
  - https://www.postman.com/mastercard/workspace/mastercard-developers/overview

### 3.2 Payments & Contactless Fundamentals

- EMVCo：
  - https://www.emvco.com/
- Stripe Tap to Pay：
  - https://docs.stripe.com/terminal/payments/setup-reader/tap-to-pay
- Google Pay Tap to Pay overview：
  - https://developers.google.com/pay/issuers/tap-to-pay

### 3.3 移动端与 NFC 相关

- Flutter：
  - https://docs.flutter.dev/
- React Native：
  - https://reactnative.dev/docs/getting-started
- Android NFC basics：
  - https://developer.android.com/develop/connectivity/nfc
- Android Host Card Emulation (HCE)：
  - https://developer.android.com/develop/connectivity/nfc/hce

### 3.4 Web 前端

- React：
  - https://react.dev/learn
- Next.js：
  - https://nextjs.org/docs
- Vue：
  - https://vuejs.org/guide/introduction.html
- Tailwind CSS：
  - https://tailwindcss.com/docs
- Recharts：
  - https://recharts.org/
- Chart.js：
  - https://www.chartjs.org/docs/latest/
- TanStack Table：
  - https://tanstack.com/table/latest

### 3.5 后端与 API

- Node.js：
  - https://nodejs.org/en/docs
- Express：
  - https://expressjs.com/
- FastAPI：
  - https://fastapi.tiangolo.com/
- ASP.NET Core：
  - https://learn.microsoft.com/en-us/aspnet/core/
- Microsoft REST API design guidelines：
  - https://github.com/microsoft/api-guidelines

### 3.6 Auth & Role-Based Access

- Auth0 docs：
  - https://auth0.com/docs
- Clerk docs：
  - https://clerk.com/docs
- JWT introduction：
  - https://jwt.io/introduction
- Auth0 RBAC：
  - https://auth0.com/docs/manage-users/access-control/rbac

### 3.7 数据库

- PostgreSQL：
  - https://www.postgresql.org/docs/
- Supabase：
  - https://supabase.com/docs
- Prisma ORM：
  - https://www.prisma.io/docs

### 3.8 Webhooks & Real-Time Dashboards

- webhooks.fyi，关注 webhook signing、retries、idempotency：
  - https://webhooks.fyi/
- ngrok，用于本地开发时暴露 localhost 接收 sandbox webhooks：
  - https://ngrok.com/docs
- Socket.IO，用于 dashboard 实时推送：
  - https://socket.io/docs/v4/

### 3.9 Accessibility, Internationalisation & Multi-Currency

- WCAG at a glance：
  - https://www.w3.org/WAI/standards-guidelines/wcag/
- WebAIM Contrast Checker：
  - https://webaim.org/resources/contrastchecker/
- i18next：
  - https://www.i18next.com/
- FormatJS / react-intl：
  - https://formatjs.io/docs/getting-started/installation/
- MDN Intl.NumberFormat：
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/NumberFormat
- ISO 4217 currency codes：
  - https://www.iso.org/iso-4217-currency-codes.html

### 3.10 文档、图表、导出

- C4 model：
  - https://c4model.com/
- Mermaid：
  - https://mermaid.js.org/
- Excalidraw：
  - https://excalidraw.com/
- draw.io：
  - https://app.diagrams.net/
- makeareadme.com：
  - https://www.makeareadme.com/
- Papa Parse，用于 CSV export：
  - https://www.papaparse.com/
- pdfmake，用于 PDF export：
  - http://pdfmake.org/
- jsPDF，用于 PDF export：
  - https://github.com/parallax/jsPDF

## 4. AI 辅助编码规则

- 2026 比赛目标是奖励能快速解决现实问题、快速创建 prototype / proof-of-concept app 的开发者。
- PDF 明确说 2026 年预计会不可避免地涉及 AI-assisted development。
- 可以使用 AI，而且官方说实际上预计你会使用 AI。
- 不需要给 AI 生成或 AI 辅助的代码添加 attribution / comment。
- 理由：AI 生成代码是你的 prompt 和已有工作的结果，AI 不拥有代码；强行注释 AI 代码会让文件混乱。
- 使用 AI 不会被扣分，前提是你理解 AI 帮你写出的代码。
- VIVA 中可能被要求解释代码的某些部分。
- 如果能完整解释代码逻辑，使用 AI 没有惩罚，也不需要披露哪些代码由 AI 写成。
- 必须检查 AI 生成代码或网上代码样例的正确性与安全性。
- 代码混乱、不安全或无法验证会被扣分，不论这些代码是谁或什么工具写的。

## 5. 评分标准总览

总分：345 分。

PDF 强调：不必完成所有项，但完成越多，获胜机会越大。

分值结构：

- Core Functionality：205 分
- UI/UX：25 分
- Code Quality：35 分
- Additional Functionality/Features：80 分
- 总计：345 分

## 6. Core Functionality - 205 分

注意：带 `**` 的内容会在正式 Task Booklet 揭晓。

| 编号 | 公开名称 / 描述 | 分值 |
| --- | --- | ---: |
| M1.1 | 与 branding 相关的内容，具体细节隐藏 | 10 |
| M1.2 | 与提供给用户的 available options 相关，具体细节隐藏 | 10 |
| M1.3 | 与用户在 app 中的 user flow 相关，具体细节隐藏 | 20 |
| M1.4 | 与 user confirmation 相关，具体细节隐藏 | 20 |
| M1.5 | Multi-Currency：至少支持 3 种货币，EUR 为 primary currency | 15 |
| M1.6 | Graceful Error Handling：对错误输入或异常进行 validation 和 error handling | 15 |
| M1.7 | Accessibility：提供 text size controls，并提供 high-contrast 的 colour scheme swap | 10 |
| M2.1 | Role-Based Access Control：登录 admin tool 后，应根据 role 开放不同层级功能 | 20 |
| M2.2 | Create & Manage ...：创建、编辑、删除某种对象，并包含 required fields，具体对象隐藏 | 20 |
| M2.3 | Live Dashboard：dashboard 展示 users 活动产生的 live data | 20 |
| M2.4 | Transaction Ledger：列出 app 中所有 transactions，并支持 filter 和 sort | 15 |
| M2.5 | CSV & PDF Export：transaction ledger 可导出为 CSV 或 PDF | 10 |
| M2.6 | Reconciliation View：将来自某个 API 的 transaction records 与 app 中记录进行匹配 | 10 |
| M2.7 | Audit Log：记录每一个 admin action | 10 |

## 7. UI/UX - 25 分

| 项目 | 要求 | 分值 |
| --- | --- | ---: |
| Neat / aesthetically pleasant user interface | 不追求花哨，而是整洁、有组织、功能明确 | 10 |
| App is easy to use | 用户不应需要说明书才能使用 | 5 |
| Responsiveness | app 应同时适配 desktop 和 mobile screens | 10 |

## 8. Code Quality - 35 分

| 项目 | 要求 | 分值 |
| --- | --- | ---: |
| Code organization | 代码组织为 packages / modules / units 等 | 5 |
| Separation between presentation and logic layers | 例如使用 REST API model，将表现层和逻辑层分离 | 10 |
| Programming paradigm | 一致、正确地使用某种编程范式，例如 OOP、AOP、functional 等 | 5 |
| Function cohesion | 函数保持小而专注，只做一件事，避免过度依赖其他函数 | 5 |
| Inline documentation | 合理添加 comments | 5 |
| Maintainable code | 使用抽象类、接口、函数原型等，取决于所选范式 | 5 |

## 9. Additional Functionality / Features - 80 分

注意：S1.1、S1.2、S1.3 中有部分正式内容被隐藏，会在 Task Booklet 揭晓。

| 编号 | 公开名称 / 描述 | 分值 |
| --- | --- | ---: |
| S1.1 | 与用户某个 action 之后的 extra actions 相关，具体细节隐藏 | 10 |
| S1.2 | 某个 additional feature 的 UI prototype，具体功能隐藏 | 10 |
| S1.3 | 某个 UI feature 的更完整 functional prototype，具体功能隐藏 | 20 |
| C1.1 | Mobile App：mobile app prototype | 15 |
| C2.1 | Multilingual UI：支持 UI translations，至少包含一种其他语言的 partial translation | 15 |
| C3.1 | Real-time dashboard：admin dashboard 实时更新 | 10 |
| Additional features | 只作为 tie-break 使用，见下方说明 | 不直接计入常规评分 |

## 10. Additional Features 的特殊规则

- 可以自由添加超出题目要求和建议的功能。
- 但 PDF 明确说这些额外功能不会被评分。
- 只有当两个提交获得完全相同分数时，additional features 才会被考虑。
- 平局时获胜者会通过 VIVA 和额外功能共同决定。
- 最终解释权由 judging panel 单独决定。

## 11. 提交要求

PDF 特别强调必须非常仔细阅读本节。

必须提交 demonstration video：

- 视频必须展示你实现的每一个功能。
- 视频必须覆盖 app 的所有功能。
- 如果有 backend，也必须展示 backend 的功能。
- 视频最好由本人旁白讲解。
- 没有提交视频会立即被取消资格。
- 任何已实现但没有在视频中展示的功能不会被评分。
- 这条规则也适用于 optional / non-core / additional features。

代码提交要求：

- 必须向评审提交代码。
- 代码、assets 和其他 resources 必须以 folder 或 compressed archive 的形式提交。
- 提交链接会由 organisers 在比赛结束时提供。
- 记得把 demonstration video 放进提交内容中。

## 12. 规则与纪律

1. 参赛资格：
   - CodeSprintMT 面向居住在 Maltese Islands 且会写代码的人开放。
   - 包括 student、graduate、working professional、educator、hobbyist、self-taught coder。
   - 参赛资格以成功注册并被 organisers 正式接受为准。
   - organisers 对接受参赛者有最终裁量权。

2. 技术栈：
   - 参赛者可以自由使用任何技术栈。
   - 包括熟悉的 programming languages、frameworks、libraries、tools。

3. 比赛地点与设备：
   - 比赛为线下 in-person。
   - 地点：ICE Campus (Zebbug)。
   - BYOD，即自带设备。
   - 会提供 internet access 和可选的 extended monitor。
   - 参赛者需要确保自己的设备能正常工作。
   - 参赛者需要提前安装所需软件和工具。
   - 参赛者需要准备连接 extended monitor 的必要 cable。

4. 个人赛与作弊：
   - 所有参赛者单独完成任务，是 solo challenge。
   - 比赛期间会有严格 security protocols。
   - 任何 plagiarise 或从其他人那里获得帮助的尝试都会导致立即取消资格。

5. 比赛环境：
   - 参赛者必须保持尊重他人的环境。
   - 需要尽量降低噪音。
   - 避免不必要的交谈。
   - 不得打扰其他参赛者。
   - 比赛房间内需要保持 silence，除非是在与 organiser 或 judge 交流。

6. AI 使用：
   - 允许负责任地使用 AI tools。
   - 不需要对 AI-generated sections 添加 comment 或 attribution。
   - 参赛者必须理解自己的代码。
   - VIVA 中可能被要求解释代码。
   - messy、insecure 或 unverifiable code 会被扣分。
   - 完整说明见 AI-Assisted Coding 部分。

7. 比赛期间必须做到：
   - 保持健康习惯，适当短暂休息。
   - 定期保存并备份工作。
   - 遵守 organisers 和 invigilators 的所有指示。
   - 在 5.00PM 前提交任务，包括 completed solution 和 demonstration video。

8. 赛后流程：
   - 所有提交会由 judging panel 评审。
   - 排名前 10 的提交会进入 VIVA shortlist。
   - VIVA 会在比赛后几天在线举行。
   - 入围者会通过 email 收到通知和 scheduled time slot。

9. 视频规则再次强调：
   - 不提交 demonstration video 会立即取消资格。
   - 视频中没有展示的功能会被评委忽略，不参与评分。

10. 额外功能规则再次强调：
   - 超出 task booklet 要求的 additional features 不会被常规评分。
   - 只有完全平分时，才结合 VIVA 和 additional features 决定。
   - 最终由 judging panel 单独裁量。

11. CCTV：
   - 比赛区域会全程 CCTV 监控。
   - 目的是 security 和 integrity。
   - 录像只会在这些目的所需期间保留。

12. 活动照片和视频：
   - 活动期间会拍摄照片和视频，用于 marketing 和 recap。
   - 不希望出现在 marketing content 中的参赛者，可以在比赛开始前通知 organisers。
   - organisers 会采取合理措施配合。

## 13. Terms and Conditions

1. Right to cancel or modify：
   - 如果出现问题导致 challenge 无法按计划运行，CodeSprintMT 保留 cancel、suspend 或 modify challenge 的权利。

2. Release：
   - 所有参赛者同意 release and hold CodeSprintMT harmless，免于与 challenge / event 相关的 claims。

3. Limitation of liability：
   - CodeSprintMT 不对技术错误或其他导致 challenge 无法按计划运行的问题负责。

4. Right to substitute：
   - 如果 advertised prize 不可用，CodeSprintMT 保留用其他奖品替代的权利。

5. Permission to record online VIVA sessions：
   - CodeSprintMT 保留录制 online VIVA sessions 的权利。
   - 录制内容仅作为 grading purposes 的证据。

6. Permission to store participants' work：
   - CodeSprintMT 保留存储参赛者提交作品最长 10 年的权利，用于 records purposes。

7. Disqualification：
   - 如果 organisers 合理认为参赛者试图破坏比赛按 Contest Rules & Regulations 的正常运行，参赛者可能被取消资格，并失去可能获得的奖项。
   - 可以联系主办方举报其他参赛者违反这些 terms。

## 14. 从已公开信息推断的正式题方向

以下不是 PDF 明确公布的完整题目，而是基于资源列表和评分表的合理推断：

- 正式题很可能与 donation / payment / transaction flow 有关。
- Mastercard Donate API 很可能是关键外部 API 或 sandbox integration。
- 可能需要用户端完成某种操作流程，并产生 transaction records。
- 可能需要 admin tool：
  - 登录
  - 角色权限
  - 创建 / 编辑 / 删除某类业务对象
  - 查看实时活动数据
  - 查看 transaction ledger
  - 导出 CSV / PDF
  - 对账
  - 查看 audit log
- 可能需要支持多币种，至少 3 种，EUR 是主币种。
- 可能需要移动端 prototype 或移动端相关设计。
- Contactless、Tap to Pay、NFC、HCE 资源说明：移动端或非接触式支付概念可能相关，但正式要求尚未公开。
- Webhooks、ngrok、Socket.IO 说明：外部 API 回调和实时 dashboard 可能是高价值准备点。
- Accessibility 和 high-contrast 不是锦上添花，而是 M1.7 的明确得分项。
- Multilingual UI 是可得分的 additional feature，至少需要一个其他语言的 partial translation。

## 15. 实作优先级建议

如果按得分和风险排序，建议优先级如下：

1. 必须先确保 app 能稳定运行在评委电脑上。
2. 必须准备 demonstration video，并逐项展示所有已实现功能。
3. 优先做 Core Functionality，尤其是 M1.5 到 M2.7 中已经公开的项目。
4. 建议采用 Web app + backend API + database 的结构，因为评分表明确看重 presentation / logic separation。
5. Admin tool 要尽早规划，因为 RBAC、dashboard、ledger、export、reconciliation、audit log 都围绕后台展开。
6. Transaction ledger 要设计为 filterable、sortable，并能导出 CSV / PDF。
7. Audit log 要记录 every admin action，不要只记录部分操作。
8. Error handling、accessibility、responsive design 属于明确得分项，不要最后才补。
9. 如果做 real-time dashboard，最好让 admin dashboard 真正实时更新，而不是只手动刷新。
10. 额外功能只有平分时有用，不应牺牲核心评分项去做花活。

## 16. 最终提交检查清单

- [ ] App 能在评委电脑上运行。
- [ ] 已准备 binary / executable solution。
- [ ] 已包含完整 source code。
- [ ] 已包含所有 assets 和 resources。
- [ ] 已打包成 folder 或 compressed archive。
- [ ] 已录制 demonstration video。
- [ ] 视频展示了每一个已实现功能。
- [ ] 视频展示了 app 功能。
- [ ] 视频展示了 backend 功能，如果实现了 backend。
- [ ] 视频最好有本人旁白。
- [ ] 视频包含 optional / non-core / additional features，否则这些功能不会评分。
- [ ] 在 5.00PM 前提交 completed solution 和 demonstration video。
- [ ] 提交内容中包含 demonstration video。
- [ ] 代码可解释，准备好 VIVA。
- [ ] AI 生成或辅助的代码已检查正确性和安全性。
- [ ] 没有依赖只有自己机器才有的隐藏配置。
- [ ] 已定期备份，避免现场丢失工作。

## 17. 逐页覆盖确认

- Page 1：封面。
- Page 2：目录。
- Page 3：欢迎与比赛目标。
- Page 4：技术总览、平台、开发环境。
- Page 5：Mastercard Sandbox、payments、contactless、移动端和 NFC 资源。
- Page 6：Web、backend、auth / RBAC、database 资源。
- Page 7：Prisma、webhooks、real-time dashboards、accessibility、i18n、multi-currency、diagram、README、CSV / PDF export 资源。
- Page 8：jsPDF。
- Page 9：AI-assisted coding 规则。
- Page 10：评分标准第一页，Core Functionality 与 UI/UX 开始。
- Page 11：评分标准第二页，UI/UX、Code Quality、Additional Functionality / Features、additional features 说明。
- Page 12：提交要求，尤其是 demonstration video 和未展示功能不评分。
- Page 13：规则 1-10 的前半部分。
- Page 14：规则 10 后半部分、CCTV、活动照片视频。
- Page 15：Terms and Conditions。
