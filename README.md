# Awesome Self-Healing Test Automation 🤖✨

<p align="center">
  <img src="assets/banner.svg" alt="Awesome Self-Healing Test Automation Banner" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a><a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Self-Healing-Test-Automation/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Self-Healing-Test-Automation?style=social" alt="GitHub stars" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Self-Healing-Test-Automation/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Self-Healing-Test-Automation?style=social" alt="GitHub forks" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Self-Healing-Test-Automation/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-CC0_1.0-blue.svg?style=flat-square" alt="License: CC0-1.0" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Self-Healing-Test-Automation/pulls"><img src="https://img.shields.io/badge/PRs-Welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome" /></a>
</p>

> 🚀 **A curated directory of top Self-Healing Test Automation tools and frameworks** — spanning cutting-edge hosted enterprise SaaS platforms and leading open-source libraries that autonomously repair brittle UI locators, adapt to DOM changes, eliminate flaky tests, and slash QA maintenance overhead.

---

## 📑 Table of Contents
- [🌐 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [🟦 SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [SaaS Products Detailed Breakdown](#-saas-products-detailed-breakdown)
- [🟩 Open-Source Software](#-open-source-software)
  - [Open-Source Repositories Detailed Breakdown](#-open-source-repositories-detailed-breakdown)
- [📊 Comparison at a Glance](#-comparison-at-a-glance)
- [🎯 Selection Guide & Best Practices](#-selection-guide--best-practices)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 🌐 Sector Overview & Market Dynamics

The global automated software testing market is estimated at **$25.1B–$32.7B**, with the dedicated **AI-driven test automation and self-healing subsector projected to surge past $8.8B** at an aggressive CAGR exceeding **22%**. 

Market concentration follows a **hybrid structure**: the broader landscape remains **moderately fragmented** with dozens of nimble startups and open-source projects innovating rapidly in generative AI and vision-based locators, while high-value enterprise testing remains **concentrated** among established quality-engineering giants (such as BrowserStack, Tricentis, Applitools/Thoma Bravo, and Katalon) through extensive M&A and bundled end-to-end testing cloud platforms.

---

## 🟦 SaaS / Hosted Platforms

The following table benchmarks leading commercial, cloud-hosted Self-Healing Test Automation platforms. The table is **sorted descending by company scale** (valuation / annual revenue).

| Platform 🏢 | Company Scale (Valuation / Revenue) 📈 | Pricing (Starting Tier) 💳 | Free Tier Limits / Free Trial 🎁 | Healing Core Tech 🧠 | Target Frameworks 🛠️ |
|:---|:---|:---|:---|:---|:---|
| **[BrowserStack](https://www.browserstack.com/)** | **~$4.0B Valuation** (~$230M ARR) | **$59/mo** (Chrome Automate, billed annually) / **$99/mo** (Desktop Automate) | **Free Trial:** 100 minutes of automated testing on real desktop/mobile browsers | Context-aware DOM history & fix-back PR automation via SDK/MCP | Selenium, Cypress, Playwright, Puppeteer |
| **[Testim](https://www.testim.io/)** *(Tricentis)* | **~$1.5B+ Valuation** (Parent Tricentis) | **~$450/mo** (Entry-level paid parallel slot tier) | **Free Trial:** 14-day free trial with AI smart locators and test authoring; No permanent free tier | AI/ML dynamic multi-attribute scoring & auto-adaptation | Web, Mobile, Salesforce |
| **[mabl](https://www.mabl.com/)** | **~$360M Valuation** (~$25M–$35M ARR) | **~$450/mo** (Core automation tier, billed annually) | **Free Trial:** 14-day full platform free trial; No permanent free tier | Historical element tracking with GenAI semantic fallback | End-to-end Web, Mobile Web, APIs |
| **[Applitools](https://applitools.com/)** | **~$250M Valuation** (Acquired by Thoma Bravo) | **$667/mo** (Starter Plan billed annually at $8,004/yr) | **Free Forever Tier:** 100 visual/checkpoint test runs per month; 14-day trial for enterprise | Visual AI & Execution Cloud DOM self-healing | Selenium, WebdriverIO, Cypress, Playwright |
| **[Leapwork](https://www.leapwork.com/)** | **~$250M–$312M Valuation** (~$35M–$38M ARR) | **~$1,833/mo** (Enterprise annual contract starting at ~$22,000/yr) | **Free Trial:** 30-day enterprise evaluation trial; No permanent free tier | Visual no-code flow with cross-referenced DOM/visual healing | Enterprise Playwright, Web, Desktop, SAP |
| **[Functionize](https://www.functionize.com/)** | **~$164M Valuation** (~$17M–$38M ARR) | **$20/mo** (Growth Plan, 3.2M execution credits/mo) / **$100/mo** (Scale Plan) | **Free Forever Tier:** $0/mo including 800,000 credits/mo for test creation & initial runs | Deep learning root-cause analysis with Smart Fix suggestions | Web, Mobile Web, Cloud Native Apps |
| **[ACCELQ](https://www.accelq.com/)** | **~$30M–$67M ARR** (~$200K Seed / Bootstrapped) | **~$350/mo** (Entry-level modular automation subscription) | **Free Trial:** 14-day full-access free trial (sample projects, cloud devices, no CC required) | Continuous DOM data calibration with contextual assertion safety | Web, Mobile, API, Packaged Apps |
| **[testRigor](https://testrigor.com/)** | **~$10M–$15M ARR** (~$5.1M Total Funding) | **$1,800/mo** (Private Tier starting base with dedicated parallel infrastructure) | **Free Forever Tier:** Unlimited tests & users for public open-source projects; 14-day trial for private | Plain-English NLP step generator with multi-step auto-adaptation | Web, Mobile (iOS/Android), Native APIs |

---

### 🔍 SaaS Products Detailed Breakdown

#### 1. BrowserStack Self-Healing Agent 🌐
- **Architecture:** AI-powered locator recovery engine integrated within BrowserStack Automate.
- **Key Capabilities:** Analyzes DOM ancestry, attributes, and proximity maps from prior passing runs. When an element identifier breaks, it synthesizes resilient locators on-the-fly and generates permanent pull requests (fix-back workflow) via SDK or MCP.
- **Best Suited For:** Engineering teams running large-scale Selenium or Cypress grids seeking enterprise stability and permanent codebase remediation.

#### 2. Testim Self-Healing (Tricentis) ⚡
- **Architecture:** Multi-attribute AI/ML locator weighting engine.
- **Key Capabilities:** Captures hundreds of attributes per element, weighting them dynamically so tests execute reliably even when class names, IDs, or element hierarchies shift.
- **Best Suited For:** Fast-moving teams maintaining complex dynamic web apps and Salesforce implementations.

#### 3. mabl Auto-Heal 🧪
- **Architecture:** Historical element baseline tracking with Generative AI fallback.
- **Key Capabilities:** Gathers a multi-run history of element properties across test cycles. Standard auto-heal resolves mild attribute drifts; GenAI triggers after repeated failures to identify semantic matches without masking genuine functional bugs.
- **Best Suited For:** Modern CI/CD teams desiring environment-aware healing that isolates staging adjustments from production assertions.

#### 4. Applitools Execution Cloud 👁️
- **Architecture:** Visual AI paired with cloud test execution infrastructure.
- **Key Capabilities:** Intercepts test runner commands and uses computer vision algorithms to dynamically resolve elements on the rendered canvas even if the underlying HTML DOM undergoes a full rewrite.
- **Best Suited For:** Teams already investing in visual regression testing wanting resilient Selenium/WDIO test execution.

#### 5. Leapwork Self-Healing 🧩
- **Architecture:** Visual no-code automation engine running atop enterprise Playwright.
- **Key Capabilities:** Continuously cross-references screen captures, DOM hierarchies, and user intent to keep visual workflow automations updated through software upgrades.
- **Best Suited For:** Enterprise QA teams and non-technical domain testers operating across Web, Desktop, and ERP systems (e.g., SAP, Salesforce).

#### 6. Functionize Smart Fix 🛠️
- **Architecture:** Autonomous root-cause analysis with human-in-the-loop suggestion approval.
- **Key Capabilities:** Detects failed assertions and selector changes, automatically re-runs variations against proposed fixes, and presents one-click fixes for QA engineer sign-off.
- **Best Suited For:** Teams seeking autonomous AI healing that strictly requires developer approval before updating test baselines.

#### 7. ACCELQ Self-Healing 🔄
- **Architecture:** Adaptive element identification with safety guardrails.
- **Key Capabilities:** Enabled out of the box; automatically distinguishes between true element locator changes and intentional absence verifications (preventing false positives on negative assertions).
- **Best Suited For:** Agile enterprise teams prioritizing zero configuration overhead and end-to-end traceability.

#### 8. testRigor Auto-Adapt ✍️
- **Architecture:** Generative AI natural-language test authoring and multi-step adjustment.
- **Key Capabilities:** Parses plain-English commands (e.g., `click "Sign In"`) from the end-user perspective; automatically adapts multi-step workflows when navigation buttons or page layouts mutate.
- **Best Suited For:** Manual testers and product managers writing tests in conversational English without CSS/XPath dependencies.

---

## 🟩 Open-Source Software

The open-source self-healing test automation ecosystem features autonomous browser agents, Playwright-native AI layers, and Selenium proxy utilities. The list below is **sorted descending by GitHub star count**.

| Repository 📦 | GitHub Stars ⭐ | Primary Stack 💻 | License 📜 | Architecture Approach 🔬 |
|:---|:---|:---|:---|:---|
| **[browserbase/stagehand](https://github.com/browserbase/stagehand)** | [![GitHub stars](https://img.shields.io/github/stars/browserbase/stagehand?style=social&color=white)](https://github.com/browserbase/stagehand/stargazers) | TypeScript / Playwright | Apache-2.0 | Hybrid AI automation framework with natural language primitives (`act`, `extract`, `observe`) |
| **[Skyvern-AI/skyvern](https://github.com/Skyvern-AI/skyvern)** | [![GitHub stars](https://img.shields.io/github/stars/Skyvern-AI/skyvern?style=social&color=white)](https://github.com/Skyvern-AI/skyvern/stargazers) | Python / Playwright | AGPL-3.0 | Vision-LLM autonomous browser agent navigating complex workflows and dynamic UIs |
| **[web-infra-dev/midscene](https://github.com/web-infra-dev/midscene)** | [![GitHub stars](https://img.shields.io/github/stars/web-infra-dev/midscene?style=social&color=white)](https://github.com/web-infra-dev/midscene/stargazers) | TypeScript / Node.js | MIT | Multimodal visual AI testing agent providing `aiAct`, `aiAssert`, and visual debugging reports |
| **[OpenAdaptAI/OpenAdapt](https://github.com/OpenAdaptAI/OpenAdapt)** | [![GitHub stars](https://img.shields.io/github/stars/OpenAdaptAI/OpenAdapt?style=social&color=white)](https://github.com/OpenAdaptAI/OpenAdapt/stargazers) | Python | MIT | Open-source AI desktop/web process automation with self-healing interaction replay |
| **[tinyfish-io/agentql](https://github.com/tinyfish-io/agentql)** | [![GitHub stars](https://img.shields.io/github/stars/tinyfish-io/agentql?style=social&color=white)](https://github.com/tinyfish-io/agentql/stargazers) | Python / TypeScript | Apache-2.0 | Natural language DOM query language replacing brittle CSS/XPaths with semantic selectors |
| **[healenium/healenium-web](https://github.com/healenium/healenium-web)** | [![GitHub stars](https://img.shields.io/github/stars/healenium/healenium-web?style=social&color=white)](https://github.com/healenium/healenium-web/stargazers) | Java / Selenium | Apache-2.0 | Native client wrapper (`SelfHealingDriver`) for automated DOM tree fallback healing |
| **[healenium/healenium](https://github.com/healenium/healenium)** | [![GitHub stars](https://img.shields.io/github/stars/healenium/healenium?style=social&color=white)](https://github.com/healenium/healenium/stargazers) | Java / PostgreSQL / Docker | Apache-2.0 | Language-agnostic proxy (`hlm-proxy`) and machine learning backend for Selenium Grid |
| **[manykarim/robotframework-heal](https://github.com/manykarim/robotframework-heal)** | [![GitHub stars](https://img.shields.io/github/stars/manykarim/robotframework-heal?style=social&color=white)](https://github.com/manykarim/robotframework-heal/stargazers) | Python / Robot Framework | Apache-2.0 | Intelligent failure classification listener (locator-drift, timing, viewport, overlay) with LLM triage |
| **[Renjithnj/zero-cost-self-healing-qa](https://github.com/Renjithnj/zero-cost-self-healing-qa)** | [![GitHub stars](https://img.shields.io/github/stars/Renjithnj/zero-cost-self-healing-qa?style=social&color=white)](https://github.com/Renjithnj/zero-cost-self-healing-qa/stargazers) | Python / Playwright | MIT | Zero-token-cost self-healing using structured accessibility trees and semantic ARIA locators |
| **[headout/autoheal](https://github.com/headout/autoheal)** | [![GitHub stars](https://img.shields.io/github/stars/headout/autoheal?style=social&color=white)](https://github.com/headout/autoheal/stargazers) | TypeScript / Multi-framework | MIT | Lightweight locator healing layer connecting Playwright and Selenium to local/cloud LLMs |
| **[vinodkumar-14/ai-playwright-framework](https://github.com/vinodkumar-14/ai-playwright-framework)** | [![GitHub stars](https://img.shields.io/github/stars/vinodkumar-14/ai-playwright-framework?style=social&color=white)](https://github.com/vinodkumar-14/ai-playwright-framework/stargazers) | Python / Playwright | MIT | Local Ollama/Mistral integration dynamically repairing broken DOM elements |
| **[SACTAN/AI-powered-locator-generation](https://github.com/SACTAN/AI-powered-locator-generation)** | [![GitHub stars](https://img.shields.io/github/stars/SACTAN/AI-powered-locator-generation?style=social&color=white)](https://github.com/SACTAN/AI-powered-locator-generation/stargazers) | Java / Selenium | MIT | Exception interceptor regenerating alternative XPath selectors using local coder LLMs |

---

### 🔬 Open-Source Repositories Detailed Breakdown

#### 1. Stagehand (`browserbase/stagehand`) 🎭
- **Stack:** TypeScript & Playwright | **License:** Apache-2.0
- **Highlights:** Combines deterministic Playwright automation with AI fallback primitives. You write standard Playwright code for known stable paths, while delegating complex, flaky, or dynamically rendered DOM segments to `page.act()` and `page.observe()`.

#### 2. Skyvern (`Skyvern-AI/skyvern`) 🦚
- **Stack:** Python & Playwright | **License:** AGPL-3.0
- **Highlights:** Leverages multimodal Computer Vision and LLM agents to autonomously parse web applications, adapt to layout updates, and complete multi-page end-to-end tasks without manual locator tagging.

#### 3. Midscene.js (`web-infra-dev/midscene`) 🎬
- **Stack:** TypeScript & Node.js | **License:** MIT
- **Highlights:** Uses multimodal vision models to "see" your UI just like human testers. Integrates seamlessly into Playwright, Vitest, and Puppeteer with natural language commands (`aiAct`, `aiAssert`) and visual execution traces.

#### 4. OpenAdapt (`OpenAdaptAI/OpenAdapt`) 🔄
- **Stack:** Python | **License:** MIT
- **Highlights:** High-performance process and GUI automation library utilizing generative AI to observe, record, and re-run automation sequences with self-healing adaptation across web and desktop apps.

#### 5. AgentQL (`tinyfish-io/agentql`) 🔎
- **Stack:** Python & TypeScript | **License:** Apache-2.0
- **Highlights:** Replaces brittle CSS and XPath selectors with semantic natural language queries (e.g., `{ login_button, user_field }`). Seamlessly integrates with Playwright scripts, making tests completely immune to HTML/DOM restyling.

#### 6. Healenium (`healenium/healenium` & `healenium-web`) 🛡️
- **Stack:** Java, Selenium WebDriver, PostgreSQL, Docker | **License:** Apache-2.0
- **Highlights:** The industry-standard open-source self-healing library for Selenium. Offers a client-side wrapper (`SelfHealingDriver`) or a universal proxy (`hlm-proxy`) that intercepts `NoSuchElementException` errors, queries its ML backend for the closest DOM match, recovers the test execution, and reports updates back to developers.

#### 7. robotframework-heal (`manykarim/robotframework-heal`) 🤖
- **Stack:** Python & Robot Framework | **License:** Apache-2.0
- **Highlights:** A dedicated test listener that classifies failures into precise categories (`locator-drift`, `timing`, `viewport`, `overlay`). Applies targeted zero-LLM fixes for timing/dialog interruptions and invokes verified LLMs solely for complex locator shifts.

#### 8. Zero-Cost Self-Healing QA (`Renjithnj/zero-cost-self-healing-qa`) ⚡
- **Stack:** Python & Playwright | **License:** MIT
- **Highlights:** Provides high-speed, 100% deterministic self-healing without paying API token costs or running heavy LLMs. Uses structured accessibility trees to match target components based on ARIA roles and labels.

---

## 📊 Comparison at a Glance

| Tool / Platform | Ecosystem Type | Primary Technology Stack | Primary Self-Healing Mechanism | Self-Hosted Option | Best For |
|:---|:---|:---|:---|:---:|:---|
| **BrowserStack** | Hosted SaaS | Selenium, Cypress, Playwright | Historical Context + Fix-Back PRs | ❌ | Teams wanting managed cloud runners & PR remediation |
| **Testim** | Hosted SaaS | Web, Mobile, Salesforce | Dynamic Multi-Attribute Weighting | ❌ | Enterprise web & Salesforce regression automation |
| **mabl** | Hosted SaaS | Web, Mobile Web, APIs | History Tracking + Generative AI | ❌ | Environment-aware CI/CD regression suites |
| **Applitools** | Hosted SaaS | Selenium, Cypress, Playwright | Visual AI & Execution Cloud | ❌ | Visual regression + automated DOM resilience |
| **Leapwork** | Enterprise SaaS | Playwright, Desktop, Web | Visual Model + DOM Cross-Referencing | ❌ | Enterprise no-code testers & ERP testing |
| **Functionize** | Hosted SaaS | Web, Mobile Web | Root-Cause Analysis + Smart Fix | ❌ | Human-in-the-loop AI healing verification |
| **ACCELQ** | Hosted SaaS | Web, Mobile, API | Adaptive Identification + Guardrails | ❌ | Out-of-the-box self-healing with zero setup |
| **testRigor** | Hosted SaaS | Web, Mobile, Native | Natural Language Multi-Step Adaptation | ❌ (Private Cloud) | Plain-English tests authored by non-developers |
| **Stagehand** | Open-Source | TypeScript, Playwright | Hybrid Code + LLM Primitives | ✅ | Playwright engineers desiring AI fallback methods |
| **Skyvern** | Open-Source | Python, Playwright | Vision-LLM Autonomous Agents | ✅ | End-to-end workflows & dynamic form automation |
| **Midscene.js** | Open-Source | TypeScript, Playwright | Multimodal UI Vision Models | ✅ | Visual assertions & natural-language test steps |
| **AgentQL** | Open-Source | Python, TypeScript | Semantic Query Language | ✅ | Semantic element extraction immune to DOM shifts |
| **Healenium** | Open-Source | Java, Selenium, Postgres | ML Proxy & Tree-Matching Algorithm | ✅ | Battle-tested Selenium self-healing infrastructure |
| **robotframework-heal** | Open-Source | Python, Robot Framework | Multi-Class Triage + LLM Fallback | ✅ | Robot Framework failure triage & locator healing |

---

## 🎯 Selection Guide & Best Practices

1. **For Selenium-Heavy Codebases:**
   - **Open-Source:** [Healenium](https://github.com/healenium/healenium) provides the most battle-tested, zero-license-cost solution via its proxy server or native Java driver wrapper.
   - **Enterprise SaaS:** [BrowserStack](https://www.browserstack.com/) offers automated fix-back pull requests to update your test repository directly.

2. **For Modern Playwright Environments:**
   - **Open-Source:** [Stagehand](https://github.com/browserbase/stagehand) and [Midscene.js](https://github.com/web-infra-dev/midscene) offer state-of-the-art vision and AI-augmented locator capabilities.
   - **Semantic Extraction:** [AgentQL](https://github.com/tinyfish-io/agentql) completely eliminates CSS/XPath selectors using natural language semantic queries.

3. **For Low-Code / Non-Technical Teams:**
   - [testRigor](https://testrigor.com/) and [Leapwork](https://www.leapwork.com/) allow teams to specify and maintain complex workflows without deep programmatic selector maintenance.

---

## 🤝 Contributing

Contributions are very welcome! If you know of an open-source tool, library, or platform that should be included:

1. 🍴 Fork this repository.
2. 🌿 Create a descriptive branch (`git checkout -b add-my-tool`).
3. 📝 Add your tool in alphabetical/star-sorted order with clear technical details and links.
4. 🚀 Submit a Pull Request.

---

## 📄 License

This collection is released under the [Creative Commons Zero v1.0 Universal (CC0-1.0)](LICENSE) Public Domain Dedication. Listed third-party tools and logos belong to their respective authors and trademark holders.

---

<p align="center">
  ⭐ <b>Star this repository if you find it helpful!</b> ⭐
</p>
