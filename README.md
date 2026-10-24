# Skill-Claude

Kho lưu các skill dành cho Claude của SGE Viettrans.

Mỗi skill nằm trong một thư mục riêng ở `skills/<tên-skill>/`, bắt buộc có file `SKILL.md` ở gốc thư mục đó.

## Quy tắc ưu tiên

**`skill-router` luôn là skill ưu tiên số một.** Mỗi khi làm việc với kho này, Claude đọc `skills/skill-router/SKILL.md` trước, rồi để skill này chọn skill phù hợp cho yêu cầu (thiết kế web, viết nội dung, logistics...). Chỉ sau đó mới đọc và làm theo skill được chọn. Quy tắc này cũng nằm trong `CLAUDE.md` và `AGENTS.md` ở gốc kho để công cụ tự đọc.

## Danh sách skill

| Skill | Dùng để làm gì | Nguồn |
|---|---|---|
| [`design-taste-frontend`](skills/design-taste-frontend/SKILL.md) | Thiết kế và chỉnh giao diện web đẹp, tránh kiểu "AI làm": landing page, trang giới thiệu, bảng điều khiển | [Leonxlnx/taste-skill](https://github.com/leonxlnx/taste-skill), giấy phép MIT |
| [`impeccable`](skills/impeccable/SKILL.md) | Thiết kế, chấm điểm (critique/audit), làm đẹp, đơn giản hóa, tăng độ bền cho giao diện web và app: bố cục, chữ, màu, chuyển động, câu chữ UX, truy cập | [pbakaus/impeccable](https://github.com/pbakaus/impeccable), giấy phép Apache 2.0 |
| [`skill-router`](skills/skill-router/SKILL.md) | Quét các skill đã cài, tự gợi ý hoặc tự chọn skill phù hợp cho từng yêu cầu (lệnh `/skill-router on`). Hữu ích khi có hàng trăm skill | [pcx-wave/skill-router](https://github.com/pcx-wave/skill-router), giấy phép MIT |
| [`emil-design-eng`](skills/emil-design-eng/SKILL.md) | Triết lý của Emil Kowalski về độ tinh tế của UI, thiết kế component, quyết định chuyển động | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`animate`](skills/animate/SKILL.md) | Làm animation từ đầu, quyết định theo thứ tự để cảm giác mượt và tự nhiên | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`animate-expo`](skills/animate-expo/SKILL.md) | Làm animation cho React Native và Expo | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`animation-performance`](skills/animation-performance/SKILL.md) | Giữ animation web trong ngân sách khung hình, chỉ animate thuộc tính nhẹ | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`animation-vocabulary`](skills/animation-vocabulary/SKILL.md) | Từ điển tra ngược: mô tả mơ hồ về hiệu ứng chuyển động thành thuật ngữ chính xác | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`apple-design`](skills/apple-design/SKILL.md) | Cách Apple thiết kế giao diện và chuyển động mềm, vật lý, áp dụng cho web | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`ask-sonner`](skills/ask-sonner/SKILL.md) | Hướng dẫn Sonner, thư viện toast cho React | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`break-ui`](skills/break-ui/SKILL.md) | Thử phá giao diện bằng dữ liệu xấu nhất: tên dài, email dài, danh sách rỗng | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`find-animation-opportunities`](skills/find-animation-opportunities/SKILL.md) | Tìm chỗ trong code/UI nên có animation mà chưa có | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`improve-animations`](skills/improve-animations/SKILL.md) | Khảo sát code animation và đề xuất danh sách cải thiện theo ưu tiên | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`mobile-native`](skills/mobile-native/SKILL.md) | Làm web app có cảm giác như app gốc trên điện thoại | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`pick-ui-library`](skills/pick-ui-library/SKILL.md) | Chọn thư viện frontend phù hợp từ danh sách chọn lọc | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`prototype`](skills/prototype/SKILL.md) | Dựng nhiều phiên bản khác nhau của một phần UI để so sánh | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`review-animations`](skills/review-animations/SKILL.md) | Rà soát code animation theo chuẩn tay nghề cao | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`write-swift`](skills/write-swift/SKILL.md) | Viết Swift hiện đại đúng chuẩn | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |

## Skill lấy từ các kho khác

Mô tả dưới đây giữ nguyên tiếng Anh của tác giả gốc. Mỗi thư mục có file `SOURCE.md` ghi kho gốc, commit và giấy phép, kèm file giấy phép nếu kho gốc có.

### andrej-karpathy-skills

Nguồn: https://github.com/forrestchang/andrej-karpathy-skills · Giấy phép: MIT (theo README và plugin.json của kho gốc)

| Skill | Mô tả |
|---|---|
| [`karpathy-guidelines`](skills/karpathy-guidelines/SKILL.md) | Behavioral guidelines to reduce common LLM coding mistakes. Use when writing, reviewing, or refactoring code to avoid ov... |

### ponytail

Nguồn: https://github.com/DietrichGebert/ponytail · Giấy phép: MIT

| Skill | Mô tả |
|---|---|
| [`ponytail`](skills/ponytail/SKILL.md) | > |
| [`ponytail-debt`](skills/ponytail-debt/SKILL.md) | > |
| [`ponytail-gain`](skills/ponytail-gain/SKILL.md) | > |
| [`ponytail-help`](skills/ponytail-help/SKILL.md) | > |
| [`ponytail-audit`](skills/ponytail-audit/SKILL.md) | > |
| [`ponytail-review`](skills/ponytail-review/SKILL.md) | > |

### caveman

Nguồn: https://github.com/JuliusBrussee/caveman · Giấy phép: Apache 2.0

| Skill | Mô tả |
|---|---|
| [`caveman`](skills/caveman/SKILL.md) | > |
| [`cavecrew`](skills/cavecrew/SKILL.md) | > |
| [`megacave`](skills/megacave/SKILL.md) | > |
| [`migration`](skills/migration/SKILL.md) | Implement reversible compatibility-safe transitions. Use for schema, data, API, protocol, configuration, or dependency m... |
| [`ultracave`](skills/ultracave/SKILL.md) | > |
| [`lean-build`](skills/lean-build/SKILL.md) | Build feature work with high overbuilding risk. Use for new behavior, product slices, or integrations where repository r... |
| [`caveman-help`](skills/caveman-help/SKILL.md) | > |
| [`caveman-learn`](skills/caveman-learn/SKILL.md) | Act on a Caveman learn report - review the ranked token sinks, apply cost-lowering fixes with per-edit consent, and repo... |
| [`caveman-setup`](skills/caveman-setup/SKILL.md) | > |
| [`caveman-stats`](skills/caveman-stats/SKILL.md) | > |
| [`safe-refactor`](skills/safe-refactor/SKILL.md) | Restructure code while preserving behavior. Use for extraction, consolidation, ownership moves, or cleanup where verific... |
| [`caveman-commit`](skills/caveman-commit/SKILL.md) | > |
| [`caveman-manage`](skills/caveman-manage/SKILL.md) | > |
| [`caveman-review`](skills/caveman-review/SKILL.md) | > |
| [`surgical-patch`](skills/surgical-patch/SKILL.md) | Fix bugs and small behavior changes at the narrowest responsible layer. Use when regression proof, preserved surrounding... |
| [`caveman-explore`](skills/caveman-explore/SKILL.md) | Read-only repository explorer for cold-start orientation, broad cross-file localization, or when a direct search failed.... |
| [`verify-and-stop`](skills/verify-and-stop/SKILL.md) | Prove existing work meets acceptance conditions without expanding scope. Use for validation-only tasks, completion check... |
| [`caveman-compress`](skills/caveman-compress/SKILL.md) | > |
| [`caveman-discover`](skills/caveman-discover/SKILL.md) | > |
| [`caveman-optimize`](skills/caveman-optimize/SKILL.md) | > |
| [`investigate-first`](skills/investigate-first/SKILL.md) | Diagnose ambiguous failures before editing. Use for unknown causes, intermittent behavior, performance regressions, or i... |
| [`caveman-evidence-review`](skills/caveman-evidence-review/SKILL.md) | > |

### ui-ux-pro-max-skill

Nguồn: https://github.com/nextlevelbuilder/ui-ux-pro-max-skill · Giấy phép: MIT

| Skill | Mô tả |
|---|---|
| [`uiux-brand`](skills/uiux-brand/SKILL.md) | Brand voice, visual identity, messaging frameworks, asset management, brand consistency. Activate for branded content, t... |
| [`uiux-design`](skills/uiux-design/SKILL.md) | Comprehensive design skill: brand identity, design tokens, UI styling, logo generation (55 styles, Gemini, Atlas Cloud,... |
| [`uiux-slides`](skills/uiux-slides/SKILL.md) | Create strategic HTML presentations with Chart.js, design tokens, responsive layouts, copywriting formulas, and contextu... |
| [`uiux-ui-styling`](skills/uiux-ui-styling/SKILL.md) | Create beautiful, accessible user interfaces with shadcn/ui components (built on Radix UI + Tailwind), Tailwind CSS util... |
| [`uiux-banner-design`](skills/uiux-banner-design/SKILL.md) | Design banners for social media, ads, website heroes, creative assets, and print. Multiple art direction options with op... |
| [`uiux-design-system`](skills/uiux-design-system/SKILL.md) | Token architecture, component specifications, and slide generation. Three-layer tokens (primitive→semantic→component), C... |
| [`ui-ux-pro-max`](skills/ui-ux-pro-max/SKILL.md) | UI/UX design intelligence for web, mobile, and desktop. This skill should be used when designing, building, reviewing, o... |

### anthropics/claude-cookbooks

Nguồn: https://github.com/anthropics/claude-cookbooks · Giấy phép: MIT

| Skill | Mô tả |
|---|---|
| [`cookbooks-cookbook-audit`](skills/cookbooks-cookbook-audit/SKILL.md) | Audit an Anthropic Cookbook notebook based on a rubric. Use whenever a notebook review or audit is requested. |
| [`applying-brand-guidelines`](skills/applying-brand-guidelines/SKILL.md) | This skill applies consistent corporate branding and styling to all generated documents including colors, fonts, layouts... |
| [`creating-financial-models`](skills/creating-financial-models/SKILL.md) | This skill provides an advanced financial modeling suite with DCF analysis, sensitivity testing, Monte Carlo simulations... |
| [`analyzing-financial-statements`](skills/analyzing-financial-statements/SKILL.md) | This skill calculates key financial ratios and metrics from financial statement data for investment analysis |

### prompts.chat

Nguồn: https://github.com/f/prompts.chat · Giấy phép: MIT (mã nguồn) và CC0 (nội dung prompt)

| Skill | Mô tả |
|---|---|
| [`book-translation`](skills/book-translation/SKILL.md) | Translate "The Interactive Book of Prompting" chapters and UI strings to a new language |
| [`widget-generator`](skills/widget-generator/SKILL.md) | Generate customizable widget plugins for the prompts.chat feed system |
| [`skill-lookup`](skills/skill-lookup/SKILL.md) | > |
| [`prompt-lookup`](skills/prompt-lookup/SKILL.md) | Activates when the user asks about AI prompts, needs prompt templates, wants to search for prompts, or mentions prompts.... |

### ECC (everything-claude-code), bản chọn lọc

Nguồn: https://github.com/affaan-m/ECC · Giấy phép: MIT

| Skill | Mô tả |
|---|---|
| [`accessibility`](skills/accessibility/SKILL.md) | Design, implement, and audit accessible UI to WCAG 2.2 Level AA across Web, iOS, and Android — semantic ARIA roles and l... |
| [`frontend-a11y`](skills/frontend-a11y/SKILL.md) | Accessibility patterns for React and Next.js — semantic HTML, ARIA attributes, form labeling, keyboard navigation, focus... |
| [`frontend-design-direction`](skills/frontend-design-direction/SKILL.md) | Set an ECC-specific frontend design direction for production UI work. Use when building or improving websites, dashboard... |
| [`frontend-patterns`](skills/frontend-patterns/SKILL.md) | Frontend development patterns for React, Next.js, state management, performance optimization, and UI best practices. Use... |
| [`frontend-slides`](skills/frontend-slides/SKILL.md) | Create stunning, animation-rich HTML presentations from scratch or by converting PowerPoint files. Use when the user wan... |
| [`design-system`](skills/design-system/SKILL.md) | Generate a design system from an existing codebase or audit one for visual consistency: extract tokens (colors, typograp... |
| [`brand-voice`](skills/brand-voice/SKILL.md) | Build a source-derived writing style profile from real posts, essays, launch notes, docs, or site copy, then reuse that... |
| [`brand-discovery`](skills/brand-discovery/SKILL.md) | Run a structured, resumable multi-session brand identity interview across 8 modules (purpose, positioning, audience, per... |
| [`article-writing`](skills/article-writing/SKILL.md) | Write articles, guides, blog posts, tutorials, newsletter issues, and other long-form content in a distinctive voice der... |
| [`content-engine`](skills/content-engine/SKILL.md) | Create platform-native content systems for X, LinkedIn, TikTok, YouTube, newsletters, and repurposed multi-platform camp... |
| [`seo`](skills/seo/SKILL.md) | Audit, plan, and implement SEO improvements across technical SEO, on-page optimization, structured data, Core Web Vitals... |
| [`market-research`](skills/market-research/SKILL.md) | Conduct market research, competitive analysis, investor due diligence, and industry intelligence with source attribution... |
| [`deep-research`](skills/deep-research/SKILL.md) | Produce cited research reports from multiple web sources using firecrawl and exa MCP tools — plan sub-questions, search... |
| [`browser-qa`](skills/browser-qa/SKILL.md) | Run automated post-deploy UI verification with a browser automation MCP (claude-in-chrome, Playwright, or Puppeteer): co... |
| [`e2e-testing`](skills/e2e-testing/SKILL.md) | Playwright E2E testing patterns, Page Object Model, configuration, CI/CD integration, artifact management, and flaky tes... |
| [`git-workflow`](skills/git-workflow/SKILL.md) | Git workflow patterns including branching strategies, commit conventions, keeping history clean and readable, tidying lo... |
| [`github-ops`](skills/github-ops/SKILL.md) | GitHub repository operations, automation, and management. Issue triage, PR management, CI/CD operations, release managem... |
| [`security-review`](skills/security-review/SKILL.md) | Use this skill when adding authentication, handling user input, working with secrets, creating API endpoints, or impleme... |
| [`documentation-lookup`](skills/documentation-lookup/SKILL.md) | Use up-to-date library and framework docs via Context7 MCP instead of training data. Activates for setup questions, API... |
| [`make-interfaces-feel-better`](skills/make-interfaces-feel-better/SKILL.md) | Apply concrete design-engineering details that make interfaces feel polished. Use when reviewing or improving UI spacing... |
| [`motion-foundations`](skills/motion-foundations/SKILL.md) | Motion tokens, spring presets, performance rules, device adaptation, accessibility enforcement, and SSR safety for React... |
| [`motion-patterns`](skills/motion-patterns/SKILL.md) | Production-ready animation patterns for React / Next.js — button, modal, toast, stagger, page transitions, exit animatio... |
| [`email-ops`](skills/email-ops/SKILL.md) | Evidence-first mailbox triage, drafting, send verification, and sent-mail-safe follow-up workflow for ECC. Use when the... |
| [`social-publisher`](skills/social-publisher/SKILL.md) | Agent-driven scheduling and publishing of social media posts across 13 platforms via SocialClaw. Use when the user wants... |
| [`marketing-campaign`](skills/marketing-campaign/SKILL.md) | End-to-end marketing campaign planning and execution. Covers audience research, positioning, campaign angle definition,... |
| [`logistics-exception-management`](skills/logistics-exception-management/SKILL.md) | Codified freight-exception handling expertise for shipment delays, damages, losses, shortages, and carrier disputes, wit... |
| [`carrier-relationship-management`](skills/carrier-relationship-management/SKILL.md) | Manage truckload, LTL, and intermodal carrier portfolios: sourcing and FMCSA vetting, freight rate and fuel-surcharge ne... |
| [`customs-trade-compliance`](skills/customs-trade-compliance/SKILL.md) | Codified customs and trade compliance expertise — HS/HTS tariff classification with GRI rules, commercial invoices and e... |
| [`inventory-demand-planning`](skills/inventory-demand-planning/SKILL.md) | Codified demand planning expertise for multi-location retailers: demand forecasting method selection, ABC/XYZ segmentati... |
| [`returns-reverse-logistics`](skills/returns-reverse-logistics/SKILL.md) | Codified expertise for returns authorization, receipt and inspection, disposition decisions, refund processing, fraud de... |

### awesome-claude-skills (Composio), bản tuyển chọn

Nguồn: https://github.com/ComposioHQ/awesome-claude-skills · Giấy phép: Apache 2.0 (theo README của kho gốc; từng skill có thể có giấy phép riêng, xem trong thư mục skill nếu có)

| Skill | Mô tả |
|---|---|
| [`artifacts-builder`](skills/artifacts-builder/SKILL.md) | Suite of tools for creating elaborate, multi-component claude.ai HTML artifacts using modern frontend web technologies (... |
| [`brand-guidelines`](skills/brand-guidelines/SKILL.md) | Applies Anthropic's official brand colors and typography to any sort of artifact that may benefit from having Anthropic'... |
| [`canvas-design`](skills/canvas-design/SKILL.md) | Create beautiful visual art in .png and .pdf documents using design philosophy. You should use this skill when the user... |
| [`changelog-generator`](skills/changelog-generator/SKILL.md) | Automatically creates user-facing changelogs from git commits by analyzing commit history, categorizing changes, and tra... |
| [`competitive-ads-extractor`](skills/competitive-ads-extractor/SKILL.md) | Extracts and analyzes competitors' ads from ad libraries (Facebook, LinkedIn, etc.) to understand what messaging, proble... |
| [`content-research-writer`](skills/content-research-writer/SKILL.md) | Assists in writing high-quality content by conducting research, adding citations, improving hooks, iterating on outlines... |
| [`developer-growth-analysis`](skills/developer-growth-analysis/SKILL.md) | Analyzes your recent Claude Code chat history to identify coding patterns, development gaps, and areas for improvement,... |
| [`domain-name-brainstormer`](skills/domain-name-brainstormer/SKILL.md) | Generates creative domain name ideas for your project and checks availability across multiple TLDs (.com, .io, .dev, .ai... |
| [`file-organizer`](skills/file-organizer/SKILL.md) | Intelligently organizes your files and folders across your computer by understanding context, finding duplicates, sugges... |
| [`image-enhancer`](skills/image-enhancer/SKILL.md) | Improves the quality of images, especially screenshots, by enhancing resolution, sharpness, and clarity. Perfect for pre... |
| [`internal-comms`](skills/internal-comms/SKILL.md) | A set of resources to help me write all kinds of internal communications, using the formats that my company likes to use... |
| [`invoice-organizer`](skills/invoice-organizer/SKILL.md) | Automatically organizes invoices and receipts for tax preparation by reading messy files, extracting key information, re... |
| [`langsmith-fetch`](skills/langsmith-fetch/SKILL.md) | Debug LangChain and LangGraph agents by fetching execution traces from LangSmith Studio. Use when debugging agent behavi... |
| [`lead-research-assistant`](skills/lead-research-assistant/SKILL.md) | Identifies high-quality leads for your product or service by analyzing your business, searching for target companies, an... |
| [`mcp-builder`](skills/mcp-builder/SKILL.md) | Guide for creating high-quality MCP (Model Context Protocol) servers that enable LLMs to interact with external services... |
| [`meeting-insights-analyzer`](skills/meeting-insights-analyzer/SKILL.md) | Analyzes meeting transcripts and recordings to uncover behavioral patterns, communication insights, and actionable feedb... |
| [`raffle-winner-picker`](skills/raffle-winner-picker/SKILL.md) | Picks random winners from lists, spreadsheets, or Google Sheets for giveaways, raffles, and contests. Ensures fair, unbi... |
| [`skill-creator`](skills/skill-creator/SKILL.md) | Guide for creating effective skills. This skill should be used when users want to create a new skill (or update an exist... |
| [`skill-share`](skills/skill-share/SKILL.md) | A skill that creates new Claude skills and automatically shares them on Slack using Rube for seamless team collaboration... |
| [`slack-gif-creator`](skills/slack-gif-creator/SKILL.md) | Toolkit for creating animated GIFs optimized for Slack, with validators for size constraints and composable animation pr... |
| [`tailored-resume-generator`](skills/tailored-resume-generator/SKILL.md) | Analyzes job descriptions and generates tailored resumes that highlight relevant experience, skills, and achievements to... |
| [`template-skill`](skills/template-skill/SKILL.md) | Replace with description of the skill and when Claude should use it. |
| [`theme-factory`](skills/theme-factory/SKILL.md) | Toolkit for styling artifacts with a theme. These artifacts can be slides, docs, reportings, HTML landing pages, etc. Th... |
| [`twitter-algorithm-optimizer`](skills/twitter-algorithm-optimizer/SKILL.md) | Analyze and optimize tweets for maximum reach using Twitter's open-source algorithm insights. Rewrite and edit user twee... |
| [`video-downloader`](skills/video-downloader/SKILL.md) | Download YouTube videos with customizable quality and format options. Use this skill when the user asks to download, sav... |
| [`webapp-testing`](skills/webapp-testing/SKILL.md) | Toolkit for interacting with and testing local web applications using Playwright. Supports verifying frontend functional... |
| [`connect-apps`](skills/connect-apps/SKILL.md) | Connect Claude to external apps like Gmail, Slack, GitHub. Use this skill when the user wants to send emails, create iss... |

### cline (skill nội bộ của kho Cline)

Nguồn: https://github.com/cline/cline · Giấy phép: Apache 2.0

| Skill | Mô tả |
|---|---|
| [`cline-opentui`](skills/cline-opentui/SKILL.md) | Comprehensive OpenTUI skill for building terminal user interfaces. Covers the core imperative API, React reconciler, and... |
| [`cline-tuistory`](skills/cline-tuistory/SKILL.md) | / |
| [`cline-sdk`](skills/cline-sdk/SKILL.md) | Comprehensive Cline SDK skill for building AI agents. Covers the Agent runtime, ClineCore sessions, custom tools, plugin... |
| [`cline-publish-cli`](skills/cline-publish-cli/SKILL.md) | Use when preparing, tagging, and publishing an apps/cli npm release. Guides changelog drafting, apps/cli/package.json ve... |
| [`cline-publish-desktop`](skills/cline-publish-desktop/SKILL.md) | Use when preparing, tagging, and publishing a Cline desktop app (apps/examples/desktop-app) release — stable (desktop-vX... |
| [`cline-desktop-whats-new`](skills/cline-desktop-whats-new/SKILL.md) | Use when the team wants to catch desktop app users up on recent features with a one-time "What's new" dialog (apps/examp... |
| [`cline-publish-extension`](skills/cline-publish-extension/SKILL.md) | Use when releasing the Cline VS Code extension — stable (standalone SDK build of main via ext-vscode-publish), nightly (... |
| [`cline-create-pull-request`](skills/cline-create-pull-request/SKILL.md) | Create a GitHub pull request following project conventions. Use when the user asks to create a PR, submit changes for re... |

### modelcontextprotocol/servers (skill nội bộ của kho MCP)

Nguồn: https://github.com/modelcontextprotocol/servers · Giấy phép: Apache 2.0 và MIT (dự án đang chuyển giấy phép, xem LICENSE)

| Skill | Mô tả |
|---|---|
| [`mcp-servers-pr-flow`](skills/mcp-servers-pr-flow/SKILL.md) | Take an issue through to a PR in this repo and close it out after merge. Use when asked to open, create or submit a PR;... |
| [`mcp-servers-release`](skills/mcp-servers-release/SKILL.md) | Cut a milestone release: the release issue, the preparation PRs on v2/main (audit, changesets Version Packages, Python C... |
| [`mcp-servers-testing`](skills/mcp-servers-testing/SKILL.md) | Write, place and run tests for a server in this repo. Use when choosing between driving the server through an MCP client... |
| [`mcp-servers-board-ops`](skills/mcp-servers-board-ops/SKILL.md) | gh recipes for the Servers V2 project board (#43): add an issue's card, move its Status, set or change its Priority, del... |
| [`mcp-servers-local-dev`](skills/mcp-servers-local-dev/SKILL.md) | Install, build and run a server from this checkout. Use when starting a server locally over stdio, SSE or Streamable HTT... |
| [`mcp-servers-client-smoke`](skills/mcp-servers-client-smoke/SKILL.md) | Drive a locally built server with a real client: the Inspector CLI (scripted), the Inspector web UI (by hand) and an LLM... |
| [`mcp-servers-issue-create`](skills/mcp-servers-issue-create/SKILL.md) | Create a tracked issue in this repo end to end — duplicate check, v2 label, type label, server-scope label, milestone, b... |
| [`mcp-servers-issue-triage`](skills/mcp-servers-issue-triage/SKILL.md) | Triage this repo's inflow — sweep unboarded issues onto the Servers V2 board (#43) as Incoming, score Priority with the... |
| [`mcp-servers-pre-push-gate`](skills/mcp-servers-pre-push-gate/SKILL.md) | Run this repo's pre-push gate and fix it when it goes red. Use when npm run local:gate fails or a stage of it does (veri... |
| [`mcp-servers-project-structure`](skills/mcp-servers-project-structure/SKILL.md) | Find where code lives in this repo's seven servers and decide where a new file goes. Use when choosing the file or direc... |
| [`mcp-servers-security-advisory`](skills/mcp-servers-security-advisory/SKILL.md) | Take a privately reported vulnerability through this repo's security advisory flow: board it as a draft card, check whet... |

### Không thêm
- `aider` (Aider-AI/aider): kho không có skill hay workflow nào dạng skill.
- `document-skills` (docx, pdf, pptx, xlsx) trong awesome-claude-skills: là skill của Anthropic dưới giấy phép riêng, không cho sao chép lại. Dùng bản có sẵn trong Claude.
- Phần lớn skill kết nối ứng dụng của Composio (hơn 800) và hơn 280 skill lập trình còn lại của ECC: chưa cần cho công ty, có thể thêm sau.

## Cách dùng với Claude

Khi muốn dùng skill, nhắn Claude đọc kho này, ví dụ: "Đọc skill trong yamy-yup/Skill-Claude rồi chỉnh giao diện trang web". Claude sẽ mở `skills/`, chọn skill phù hợp, đọc `SKILL.md` (và các file đi kèm nếu skill yêu cầu) rồi mới làm.

Dùng trong Claude Code: chép thư mục skill cần dùng vào `.claude/skills/` của dự án.

## Thêm skill mới

1. Tạo thư mục `skills/<tên-skill>/`, dùng chữ thường và dấu gạch ngang.
2. Đặt `SKILL.md` ở gốc thư mục, đầu file có phần thông tin:
   ```
   ---
   name: <tên-skill, trùng tên thư mục>
   description: <khi nào nên dùng skill này>
   ---
   ```
3. Để tài liệu, mẫu, script đi kèm trong các thư mục con (ví dụ `references/`, `scripts/`).
4. Nếu skill lấy từ nguồn khác, giữ file giấy phép (`LICENSE`) trong thư mục skill và ghi nguồn vào bảng ở trên.
5. Cập nhật bảng danh sách skill trong README này.
