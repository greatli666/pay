# CodeSprintMT 2026 Open Category Key Points

Source file: `CodeSprintMT-2026-Open-Category-Competition-Prep-Guide.pdf`

Note: this PDF is the 2026 Open Category Preparation Booklet, not the final full Task Booklet. Some final task details are intentionally hidden in the judgement criteria as `...` or `Something related to ...**`. The PDF explicitly says those items will be revealed in the task booklet. This document captures all key information that is visible in the preparation booklet and separately labels directional inferences from the resources and scoring table.

## 1. Document Structure

- Cover: Preparation Booklet, Open Category 2026.
- Table of contents:
  - Technical Overview
  - Preparation Resources
  - AI-Assisted Coding
  - Judgement Criteria
  - Submission Criteria
  - Rules and Regulations
  - Terms and Conditions
- Welcome page: participants will use coding, infrastructure, and UI/UX design skills to create an app.

## 2. Technical Overview

- During the competition, participants will design and build an app.
- The judging panel has created a reference implementation in one working day to prove that the task can be completed within the allocated time.
- A demonstration of the reference implementation will be available on competition day.
- Any platform is allowed:
  - Windows
  - macOS
  - Linux
  - Android
  - iOS
  - Web
- A web-based platform is recommended because it is usable on more platforms, but this does not affect the points awarded.
- Any programming language may be used.
- The solution must run on the judges' computers.
- Participants must provide:
  - binary / executable solution
  - source code

## 3. Preparation Resources and Technical Signals

The PDF says these resources are meant to help participants prepare for the task, and that any familiar technology may be used. The resource list strongly suggests that the final task may involve payments, donations, transactions, admin tooling, real-time data, role-based permissions, multi-currency support, exports, and reconciliation.

### 3.1 Mastercard Sandbox

- Creating a Mastercard Sandbox account:
  - https://developer.mastercard.com/donations/documentation/quick-start-guide/#generate-credentials-and-create-a-sandbox-project
- Mastercard Donate:
  - https://developer.mastercard.com/product/mastercard-donate/
- Donate API documentation:
  - https://developer.mastercard.com/donations/documentation
- Donate API reference:
  - https://developer.mastercard.com/donations/documentation/api-reference/
- Donate API basics:
  - https://developer.mastercard.com/donations/documentation/api-basics/
- Mastercard Postman workspace, recommended for calling the APIs before writing code:
  - https://www.postman.com/mastercard/workspace/mastercard-developers/overview

### 3.2 Payments & Contactless Fundamentals

- EMVCo:
  - https://www.emvco.com/
- Stripe Tap to Pay:
  - https://docs.stripe.com/terminal/payments/setup-reader/tap-to-pay
- Google Pay Tap to Pay overview:
  - https://developers.google.com/pay/issuers/tap-to-pay

### 3.3 Mobile and NFC Resources

- Flutter:
  - https://docs.flutter.dev/
- React Native:
  - https://reactnative.dev/docs/getting-started
- Android NFC basics:
  - https://developer.android.com/develop/connectivity/nfc
- Android Host Card Emulation (HCE):
  - https://developer.android.com/develop/connectivity/nfc/hce

### 3.4 Web Frontend

- React:
  - https://react.dev/learn
- Next.js:
  - https://nextjs.org/docs
- Vue:
  - https://vuejs.org/guide/introduction.html
- Tailwind CSS:
  - https://tailwindcss.com/docs
- Recharts:
  - https://recharts.org/
- Chart.js:
  - https://www.chartjs.org/docs/latest/
- TanStack Table:
  - https://tanstack.com/table/latest

### 3.5 Backend and APIs

- Node.js:
  - https://nodejs.org/en/docs
- Express:
  - https://expressjs.com/
- FastAPI:
  - https://fastapi.tiangolo.com/
- ASP.NET Core:
  - https://learn.microsoft.com/en-us/aspnet/core/
- Microsoft REST API design guidelines:
  - https://github.com/microsoft/api-guidelines

### 3.6 Auth & Role-Based Access

- Auth0 docs:
  - https://auth0.com/docs
- Clerk docs:
  - https://clerk.com/docs
- JWT introduction:
  - https://jwt.io/introduction
- Auth0 RBAC:
  - https://auth0.com/docs/manage-users/access-control/rbac

### 3.7 Database

- PostgreSQL:
  - https://www.postgresql.org/docs/
- Supabase:
  - https://supabase.com/docs
- Prisma ORM:
  - https://www.prisma.io/docs

### 3.8 Webhooks & Real-Time Dashboards

- webhooks.fyi, covering webhook signing, retries, and idempotency:
  - https://webhooks.fyi/
- ngrok, for exposing localhost to receive sandbox webhooks during development:
  - https://ngrok.com/docs
- Socket.IO, for pushing live updates to dashboards:
  - https://socket.io/docs/v4/

### 3.9 Accessibility, Internationalisation & Multi-Currency

- WCAG at a glance:
  - https://www.w3.org/WAI/standards-guidelines/wcag/
- WebAIM Contrast Checker:
  - https://webaim.org/resources/contrastchecker/
- i18next:
  - https://www.i18next.com/
- FormatJS / react-intl:
  - https://formatjs.io/docs/getting-started/installation/
- MDN Intl.NumberFormat:
  - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Intl/NumberFormat
- ISO 4217 currency codes:
  - https://www.iso.org/iso-4217-currency-codes.html

### 3.10 Diagrams, README, and Exports

- C4 model:
  - https://c4model.com/
- Mermaid:
  - https://mermaid.js.org/
- Excalidraw:
  - https://excalidraw.com/
- draw.io:
  - https://app.diagrams.net/
- makeareadme.com:
  - https://www.makeareadme.com/
- Papa Parse, for CSV export:
  - https://www.papaparse.com/
- pdfmake, for PDF export:
  - http://pdfmake.org/
- jsPDF, for PDF export:
  - https://github.com/parallax/jsPDF

## 4. AI-Assisted Coding Rules

- The 2026 competition aims to reward developers who can quickly solve real-world problems and create prototypes / proof-of-concept apps.
- The PDF states that in 2026 this will inevitably involve AI-assisted development.
- AI may be used. The PDF says it is expected.
- Participants do not need to comment or attribute AI-generated or AI-assisted sections.
- The reason given is that AI-created code is the result of the participant's prompt and existing work; the AI does not own the code, and marking AI sections would create messy code files.
- AI use is not penalised if the participant understands the generated code.
- During the VIVA, participants may be asked to explain parts of their code.
- If the participant can fully explain the code, there is no penalty for using AI and no need to disclose which parts were AI-written.
- Participants must verify AI-generated code and any traditionally sourced code samples for correctness and security.
- Messy, insecure, or unverifiable code will be penalised regardless of who or what wrote it.

## 5. Judgement Criteria Overview

Maximum score: 345 points.

The PDF states that participants do not need to achieve every criterion, but the more criteria they achieve, the better their chances of winning.

Score breakdown:

- Core Functionality: 205 points
- UI/UX: 25 points
- Code Quality: 35 points
- Additional Functionality/Features: 80 points
- Total: 345 points

## 6. Core Functionality - 205 Points

Items marked with `**` will be revealed in the task booklet.

| ID | Public name / description | Points |
| --- | --- | ---: |
| M1.1 | Something related to branding; exact detail hidden | 10 |
| M1.2 | Something related to available options available to the user; exact detail hidden | 10 |
| M1.3 | Something related to user flow through the app; exact detail hidden | 20 |
| M1.4 | Something related to user confirmation; exact detail hidden | 20 |
| M1.5 | Multi-Currency: support at least three currencies, with EUR as the primary currency | 15 |
| M1.6 | Graceful Error Handling: validation and error handling for incorrect input or exceptions | 15 |
| M1.7 | Accessibility: text size controls and a high-contrast colour scheme swap | 10 |
| M2.1 | Role-Based Access Control: logging into the admin tool should allow increasing functionality based on role | 20 |
| M2.2 | Create & Manage ...: create, edit, and delete something with required fields; exact object hidden | 20 |
| M2.3 | Live Dashboard: dashboard showing live data from activities carried out by users | 20 |
| M2.4 | Transaction Ledger: list all transactions carried out in the app; filterable and sortable | 15 |
| M2.5 | CSV & PDF Export: transaction ledger exportable as CSV or PDF | 10 |
| M2.6 | Reconciliation View: match transaction records from an API to those recorded from the app | 10 |
| M2.7 | Audit Log: log every admin action | 10 |

## 7. UI/UX - 25 Points

| Criterion | Requirement | Points |
| --- | --- | ---: |
| Neat / aesthetically pleasant user interface | The judges want a neat, organised, functional UI rather than flair | 10 |
| App is easy to use | Users should not need a manual to use the app | 5 |
| Responsiveness | The app should be usable on both desktop and mobile screens | 10 |

## 8. Code Quality - 35 Points

| Criterion | Requirement | Points |
| --- | --- | ---: |
| Code organization | Code organized into packages / modules / units etc. | 5 |
| Separation between presentation and logic layers | For example, using a REST API model | 10 |
| Programming paradigm | Consistent and correct use of a paradigm such as OOP, AOP, or functional programming | 5 |
| Function cohesion | Functions should be small, do one thing, and avoid excessive dependency on other functions | 5 |
| Inline documentation | Comments where appropriate | 5 |
| Maintainable code | Abstract classes, interfaces, function prototypes, etc., depending on the chosen paradigm | 5 |

## 9. Additional Functionality / Features - 80 Points

S1.1, S1.2, and S1.3 have hidden details that will be revealed in the task booklet.

| ID | Public name / description | Points |
| --- | --- | ---: |
| S1.1 | Something related to extra actions following a user action; exact detail hidden | 10 |
| S1.2 | A UI prototype for an additional feature; exact feature hidden | 10 |
| S1.3 | A more functional prototype for a UI feature; exact feature hidden | 20 |
| C1.1 | Mobile App: prototype of a mobile app | 15 |
| C2.1 | Multilingual UI: support UI translations, with at least one partial translation to another language | 15 |
| C3.1 | Real-time dashboard: admin dashboard updated in real time | 10 |
| Additional features | Used only as a tie-break; see below | Not part of ordinary scoring |

## 10. Special Rule for Additional Features

- Participants may add features beyond the stated requirements and suggestions.
- The PDF explicitly says these extra features will not be graded.
- Additional features are considered only if two submissions receive the exact same grade.
- In a tie, the winner is decided through the VIVA and the additional features provided.
- This decision is at the sole discretion of the judging panel.

## 11. Submission Criteria

The PDF tells participants to read this section very carefully.

A demonstration video is mandatory:

- The video must showcase each and every feature implemented in the solution.
- The video must go through all functionality of the app.
- If a backend was created, backend functionality must also be demonstrated.
- Ideally, the video should be narrated by the participant.
- Failure to submit a video results in immediate disqualification.
- Any implemented feature that is not demonstrated in the video will not be graded.
- This includes optional, non-core, and additional features.

Code submission requirements:

- Participants must submit code to the judging panel.
- Code, assets, and other resources must be submitted as a folder or compressed archive.
- The submission link will be provided by the organisers at the end of the competition.
- The demonstration video must be included in the submission.

## 12. Rules and Regulations

1. Eligibility:
   - CodeSprintMT is open to anyone residing within the Maltese Islands who codes.
   - This includes students, graduates, working professionals, educators, hobbyists, and self-taught coders.
   - Participation is confirmed after successful registration and formal acceptance by the organisers.
   - Acceptance is at the sole discretion of the organisers.

2. Tech stack:
   - Participants may use any tech stack of their choice.
   - This includes familiar programming languages, frameworks, libraries, and tools.

3. Venue and equipment:
   - The session is in-person.
   - Location: ICE Campus (Zebbug).
   - Bring-your-own-device model.
   - Internet access and an optional extended monitor will be provided.
   - Participants are responsible for ensuring that their device is fully functional.
   - Participants must pre-load any required software or tools.
   - Participants must bring the necessary cable to connect to the extended monitor.

4. Solo challenge and cheating:
   - All participants work individually.
   - The competition is a solo challenge.
   - Strict security protocols will be in place.
   - Any attempt to plagiarise or receive help from another person results in immediate disqualification.

5. Competition environment:
   - Participants must maintain a respectful environment.
   - Noise should be kept to a minimum.
   - Unnecessary conversation should be avoided.
   - Participants must not distract others.
   - Silence must be observed in the competition room unless speaking with an organiser or judge.

6. AI use:
   - Participants may use AI tools responsibly.
   - AI-generated sections do not need comments or attribution.
   - Participants must understand their own code.
   - Participants may be asked to explain code during the VIVA.
   - Messy, insecure, or unverifiable code will be penalised.
   - The full AI guidance is in the AI-Assisted Coding section.

7. Mandatory behaviour during the session:
   - Maintain healthy habits and take short breaks.
   - Save and back up work regularly.
   - Follow all instructions from organisers and invigilators.
   - Submit the task, including the completed solution and demonstration video, by 5.00PM.

8. Post-competition process:
   - All submissions will be reviewed by the judging panel.
   - The top 10 ranked submissions will be shortlisted for a VIVA.
   - The VIVA will be held online a couple of days after the competition.
   - Shortlisted participants will be notified by email and given a scheduled time slot.

9. Video rule repeated:
   - Failure to submit a demonstration video results in immediate disqualification.
   - Features not demonstrated in the video will be ignored by judges during grading.

10. Additional features rule repeated:
   - Additional features beyond the task booklet requirements are not graded normally.
   - They are considered only in a perfect tie.
   - The tie is resolved using a combination of participant VIVA and additional features.
   - The judging panel has sole discretion.

11. CCTV:
   - The competition area will be monitored by CCTV throughout the session.
   - The purpose is security and integrity.
   - Footage is retained only as long as necessary for those purposes.

12. Event photographs and videos:
   - Photographs and video recordings will be taken for marketing and recap purposes.
   - Participants who do not want to appear in marketing content may notify the organisers before the competition starts.
   - The organisers will take reasonable steps to accommodate this.

## 13. Terms and Conditions

1. Right to cancel or modify:
   - CodeSprintMT may cancel, suspend, or modify the challenge if any problem prevents it from running as planned.

2. Release:
   - All participants agree to release and hold CodeSprintMT harmless from claims associated with the challenge or event.

3. Limitation of liability:
   - CodeSprintMT is not responsible or liable for technical errors or other issues that may prevent the challenge from running as planned.

4. Right to substitute:
   - CodeSprintMT may substitute prizes if the advertised prize is not available.

5. Permission to record online VIVA sessions:
   - CodeSprintMT may record online VIVA sessions.
   - Recordings are used as evidence for grading purposes only.

6. Permission to store participants' work:
   - CodeSprintMT may store submitted participant work for up to 10 years for record purposes.

7. Disqualification:
   - A participant may be disqualified and forfeit prizes if the organiser reasonably believes the participant attempted to undermine the legitimate operation of the contest under the Contest Rules & Regulations.
   - Participants may report violations of these terms by contacting the organisers.

## 14. Inferred Direction of the Final Task

The following points are not the fully published task. They are reasonable inferences based on the visible resources and judgement criteria:

- The final task is likely connected to donation / payment / transaction flows.
- Mastercard Donate API is likely to be an important external API or sandbox integration.
- The user-facing app may need to guide users through an action flow that creates transaction records.
- An admin tool is likely important:
  - login
  - role-based access
  - create / edit / delete a hidden business object
  - live activity dashboard
  - transaction ledger
  - CSV / PDF export
  - reconciliation
  - audit log
- Multi-currency support is likely required, with at least three currencies and EUR as primary.
- A mobile prototype or mobile-related design may be valuable.
- Contactless, Tap to Pay, NFC, and HCE resources suggest that mobile or contactless payment concepts may be relevant, although the final requirement is not yet visible.
- Webhooks, ngrok, and Socket.IO suggest that external API callbacks and real-time dashboards may be high-value preparation areas.
- Accessibility and high-contrast support are explicit scoring items, not optional polish.
- Multilingual UI is a scored additional feature, requiring at least one partial translation to another language.

## 15. Implementation Priority Suggestions

Based on points and risk, the practical priority order should be:

1. Make sure the app runs reliably on the judges' computers.
2. Prepare the demonstration video and show every implemented feature.
3. Prioritise Core Functionality, especially the visible M1.5 to M2.7 items.
4. Prefer a web app + backend API + database architecture, because the criteria reward separation between presentation and logic.
5. Plan the admin tool early, because RBAC, dashboard, ledger, export, reconciliation, and audit log all depend on it.
6. Build the transaction ledger as filterable, sortable, and exportable to CSV / PDF.
7. Make the audit log record every admin action, not only selected actions.
8. Error handling, accessibility, and responsive design are explicit scoring items and should not be left until the end.
9. If building a real-time dashboard, make the admin dashboard actually update in real time rather than relying only on manual refresh.
10. Do not sacrifice core scoring items for extra features, since extras only matter in a tie.

## 16. Final Submission Checklist

- [ ] The app runs on the judges' computers.
- [ ] Binary / executable solution is prepared.
- [ ] Full source code is included.
- [ ] All assets and resources are included.
- [ ] Submission is packaged as a folder or compressed archive.
- [ ] Demonstration video is recorded.
- [ ] Video demonstrates every implemented feature.
- [ ] Video demonstrates app functionality.
- [ ] Video demonstrates backend functionality if a backend exists.
- [ ] Video is ideally narrated by the participant.
- [ ] Video includes optional / non-core / additional features if those features should be graded or considered.
- [ ] Completed solution and demonstration video are submitted by 5.00PM.
- [ ] Demonstration video is included in the submission.
- [ ] Participant can explain the code for the VIVA.
- [ ] AI-generated or AI-assisted code has been checked for correctness and security.
- [ ] No hidden local-only configuration is required to run the app.
- [ ] Work has been saved and backed up regularly.

## 17. Page-by-Page Coverage Check

- Page 1: cover.
- Page 2: table of contents.
- Page 3: welcome and competition goal.
- Page 4: technical overview, platform, development environment.
- Page 5: Mastercard Sandbox, payments, contactless, mobile, and NFC resources.
- Page 6: web, backend, auth / RBAC, and database resources.
- Page 7: Prisma, webhooks, real-time dashboards, accessibility, i18n, multi-currency, diagrams, README, CSV / PDF export resources.
- Page 8: jsPDF.
- Page 9: AI-assisted coding rules.
- Page 10: first page of judgement criteria, core functionality and beginning of UI/UX.
- Page 11: second page of judgement criteria, UI/UX, code quality, additional functionality / features, and additional features explanation.
- Page 12: submission criteria, especially the demonstration video and the rule that undemonstrated features will not be graded.
- Page 13: rules 1-10, first part.
- Page 14: rest of rule 10, CCTV, event photos and videos.
- Page 15: terms and conditions.
