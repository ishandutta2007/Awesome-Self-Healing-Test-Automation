# Awesome-Self-Healing-Test-Automation

# Awesome Self-Healing Test Automation

> A curated list of top Self-Healing Test Automation platforms — both SaaS/Hosted commercial solutions and open-source alternatives for automatically recovering from broken locators and UI changes without manual test maintenance.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [BrowserStack Self-Healing Agent](#browserstack-self-healing-agent)
  - [Testim Self-Healing](#testim-self-healing)
  - [mabl Auto-Heal](#mabl-auto-heal)
  - [Functionize Smart Fix](#functionize-smart-fix)
  - [AccelQ Self-Healing](#accelq-self-healing)
  - [Katalon Self-Healing](#katalon-self-healing)
  - [Applitools Execution Cloud](#applitools-execution-cloud)
  - [testRigor Auto-Adapt](#testrigor-auto-adapt)
  - [Leapwork Self-Healing](#leapwork-self-healing)
- [Open-Source Software](#-open-source-software)
  - [Healenium](#healenium)
  - [Aumate QA Agent](#aumate-qa-agent)
  - [robotframework-heal](#robotframework-heal)
  - [AgentQL](#agentql)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Self-Healing Test Automation platforms. These are not open-source but are included as reference points for feature comparison.

### BrowserStack Self-Healing Agent
**Type:** AI-powered locator healing within BrowserStack Automate  
BrowserStack Self-Heal uses AI to automatically recover failed tests when locators break due to UI changes. It stores element context (locator, nearby attributes, DOM structure) from successful runs, then generates resilient locators when the original fails [citation:4][citation:15]. Supported frameworks include Selenium (Java, Python, JS, C#) and Cypress (currently v15.8 only), across desktop and mobile browsers [citation:4][citation:15]. A key differentiator is the **fix-back workflow**: healed locators can be applied to test scripts via MCP or a GitHub PR through the SDK, preventing recurrence [citation:4][citation:15]. **Limitations:** Requires at least one successful execution with the same `elementIdentifier`; cannot heal system failures or WebDriver issues; may misfire on negative assertions [citation:4]. Available on Automate Pro with BrowserStack AI enabled [citation:15].  
**Best for:** Teams already running Selenium or Cypress on BrowserStack Automate wanting AI-assisted locator healing with a path to permanently fix test scripts.

### Testim Self-Healing
**Type:** AI/ML custom locators with self-healing  
Testim uses custom AI/ML locators that learn about the application and automatically self-heal as it changes, keeping tests working through UI updates [citation:5]. Positioned for Salesforce, web, and mobile testing, with smart locators that identify elements based on multiple attributes rather than relying on a single selector.

### mabl Auto-Heal
**Type:** Element history-based healing with generative AI fallback  
mabl builds an **element history** from recorded steps, tracking attributes, ancestors, and custom test IDs. During runs, it looks for strong matches first, then attempts standard auto-heal (best available match), followed by **advanced auto-heal using generative AI** to find semantic similarities when standard strategies fail [citation:6]. Healing is tracked per environment, so QA changes don't affect production behavior. Advanced auto-heal only activates after at least 5 successful plan runs [citation:6].  
**Best for:** Teams wanting a mature auto-heal system with environment-aware element tracking and generative AI as a fallback layer.

### Functionize Smart Fix
**Type:** Root cause analysis with self-heal suggestions  
Functionize's Self-Heal works alongside Smart Suggestions: when a test fails, root cause analysis generates possible fixes, and self-heal automatically re-runs the test with each suggestion, reporting results. Users approve successful resolutions, which are then applied to the test [citation:7]. This human-in-the-loop approach balances automation with control.

### AccelQ Self-Healing
**Type:** Comprehensive adaptive element identification  
AccelQ's self-healing is **on by default** for all test runs, with a rich visual interface in test reports showing the source of element flakiness [citation:8]. It explicitly skips self-healing for contextually doubtful statements (e.g., waiting for an element to disappear or verifying absence), preventing false matches. Data calibration runs continually across project runs [citation:8].

### Katalon Self-Healing
**Type:** Classic + AI self-healing with approval workflow  
Katalon Studio offers two tiers: **classic self-healing** (free) tries alternative locators in order, while **AI self-healing** (paid) uses page source, accessibility tree, and screenshots when all locators fail [citation:9]. Proposed fixes appear in **Self-healing Insights** for approval or discard, and approved locators are saved as defaults. Smart Wait (free) handles timing failures separately [citation:9].  
**Best for:** Teams wanting a clear separation between free classic healing and paid AI healing, with explicit approval before changes are applied.

### Applitools Execution Cloud
**Type:** AI self-healing within test execution cloud  
Applitools Execution Cloud provides AI-based self-healing for Selenium and WDIO tests, allowing tests to run successfully even when element locators change. It works seamlessly with the Ultrafast Grid for cross-environment verification [citation:10]. Positioned for teams already using Applitools for visual testing wanting additional resilience in test execution.

### testRigor Auto-Adapt
**Type:** AI-generated steps with auto-adaptation  
testRigor's auto-adapt enhancement (July 2025) allows the system to handle and adapt **multiple steps at once** during test generation, analyzing overall context to generate, adjust, and optimize steps simultaneously [citation:11]. When a test fails due to a typo or error, it starts self-healing and reports the steps taken to resolve it, including typo corrections and recognized intent [citation:11].

### Leapwork Self-Healing
**Type:** Cross-referenced DOM/screen/source healing  
Leapwork's self-healing cross-references the DOM, screen, and source requirements to keep tests current when applications change [citation:12]. Positioned within Leapwork's enterprise Playwright offering, extending Playwright's capabilities with vendor-managed resilience.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Self-Healing Test Automation tools. The open-source ecosystem is **led by Healenium** for Selenium-based healing, with newer entrants offering framework-agnostic and AI-assisted approaches.

### Healenium
**Stack:** Java / PostgreSQL / Selenium | **License:** Open Source (Apache-2.0)  
Healenium is the most established open-source self-healing library for Selenium-based tests, using machine learning to detect and heal failures caused by UI changes like modified element IDs or class names [citation:2]. It offers two approaches:
- **Healenium-Proxy:** Platform-agnostic, sits between the test runner and application, healing Selenium tests at the server level regardless of language (Java, Python, JS, C#) [citation:2]
- **Healenium-Web:** Java-only integration where you wrap `WebDriver` in `SelfHealingDriver` [citation:2]

Features include support for `@FindBy`/PageFactory, semantic locators (Id, Name, ClassName, LinkText, TagName), iframes, Actions, Selenide integration, parallel and remote test runs, and mobile testing via Appium adapter [citation:14]. An IntelliJ IDEA plugin updates broken locators in the codebase with one click [citation:14]. Docker deployment with PostgreSQL, hlm-proxy, hlm-backend, and Selenium Grid [citation:2].  
**Best for:** Java/Selenium teams wanting a proven, ML-based self-healing library with both proxy and native integration options, accepting the Java-centric ecosystem.

### Aumate QA Agent
**Stack:** Python | **License:** Open Source (per PyPI)  
Aumate QA Agent is a framework-agnostic auto-healing tool that observes existing tests without requiring any test code changes. It detects failures (locators, timing, assertions), collects DOM evidence, generates candidates (deterministic + optional AI), and tests each candidate in an isolated sandbox copy before applying the fix [citation:3]. **Safety guarantees** include: no LLM has direct write access (validation engine is sole gatekeeper), application defects are never hidden (only automation defects healed), and secrets are masked before sending to LLMs [citation:3]. Supports Playwright (TS/JS/Python) and Selenium (Python/Java/JS), with LLM providers including Gemini (default), OpenAI, Groq, Ollama, OpenRouter, and Azure OpenAI. Works fully offline with deterministic healing if no LLM configured [citation:3].  
**Best for:** Teams wanting framework-agnostic, zero-code-change healing with strong safety guarantees and optional LLM assistance, particularly Python/Playwright/Selenium stacks.

### robotframework-heal
**Stack:** Python / Robot Framework | **License:** Open Source (per GitHub)  
robotframework-heal is a Robot Framework listener for failure triage, self-healing, and root-cause analysis of UI tests (Browser/Playwright, SeleniumLibrary, Appium) [citation:13]. It classifies failures into distinct classes and applies targeted fixes:
- **locator-drift:** tiered deterministic candidates → LLM picks (verified live) → full-DOM fallback; iframe support via `frame >>> inner` selectors
- **timing:** waits for page-ready and reruns (no LLM)
- **viewport:** scrolls/swipe-searches element into view (no LLM)
- **overlay:** dismisses blocking dialogs/banners, verifies, reruns
- **form-state:** diagnoses unfilled required/invalid fields
- **assertion-drift:** opt-in UI text drift verification

Every failed keyword produces an enriched error record, with an HTML report at `results/heal/heal_report.html`. Supports per-role LLM overrides (triage, locator, vision, RCA) and multiple output modes [citation:13].  
**Best for:** Robot Framework teams wanting sophisticated failure classification with targeted, non-LLM fixes for timing/viewport/overlay issues and LLM assistance only where needed.

### AgentQL
**Stack:** Python / JavaScript | **License:** Open Source (free tier)  
AgentQL provides a natural language query language for AI agents to interact with and extract structured data from web pages, with **self-healing selectors** that integrate with Playwright [citation:1]. Instead of brittle CSS/XPath selectors, AgentQL queries describe elements semantically (e.g., "the login button"), making them resilient to DOM changes.  
**Best for:** Playwright teams wanting semantic, self-healing element selection via natural language queries rather than traditional locators.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Healing Approach | Framework Support | Self-Hosted | Best For |
|----------|---------|-------|------------------|-------------------|-------------|----------|
| **BrowserStack** | Proprietary | Cloud | AI locator healing | Selenium, Cypress | ❌ | BrowserStack + fix-back workflow |
| **Testim** | Proprietary | Cloud | AI/ML custom locators | Web, mobile, Salesforce | ❌ | AI locator learning |
| **mabl** | Proprietary | Cloud | Element history + GenAI | Recorded browser steps | ❌ | Environment-aware healing |
| **Functionize** | Proprietary | Cloud | Smart Fix suggestions | (Check) | ❌ | Human-in-the-loop fixes |
| **AccelQ** | Proprietary | Cloud | Adaptive identification | (Check) | ❌ | Default-on healing + visual reports |
| **Katalon** | Proprietary | Cloud/Desktop | Classic + AI tiers | Katalon Studio | (Desktop) | Free classic + paid AI |
| **Healenium** | Apache-2.0 | Java/Postgres | ML-based healing | Selenium (all langs via proxy) | ✅ | Proven OSS Selenium healing |
| **Aumate** | Open Source | Python | Deterministic + AI sandbox | Playwright, Selenium | ✅ | Zero-code-change + safety |
| **robotframework-heal** | Open Source | Python | Failure-class targeted | Robot Framework | ✅ | Sophisticated failure triage |
| **AgentQL** | Open Source | Python/JS | Semantic NL selectors | Playwright | ✅ (Library) | Natural language element queries |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Self-Healing Test Automation tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem **splits** between **Selenium-focused healing** (Healenium, the most established option with ML-based locator recovery), **framework-agnostic zero-code-change tools** (Aumate, with strong safety guarantees and optional LLM), **failure-class-specific listeners** (robotframework-heal, with targeted non-LLM fixes for timing/viewport/overlay), and **semantic selector libraries** (AgentQL, using natural language instead of CSS/XPath). Commercial platforms like BrowserStack, mabl, and Katalon offer more integrated workflows with fix-back automation and environment-aware tracking, but open-source tools now cover the core healing capability for teams willing to manage their own infrastructure.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
