# The Ultimate ChatGPT Slash Commands Handbook (2026 Edition)

<p align="center">
  <a href="https://linktr.ee/YourAKShaw" target="_blank">
    <img src="https://i.ibb.co/vvsszQmY/chatgpt-playbook-gist-cover-yourakshaw-1.png" alt="Follow AK Shaw on Linktree" />
  </a>
</p>

> **The most comprehensive community and platform reference for ChatGPT slash commands, pseudo-commands, workflow triggers, and power-user prompting systems.**

---

## Disclaimer

There is currently **no single official public OpenAI master list** containing every slash command across the entire ChatGPT ecosystem. 

Because OpenAI frequently runs regional tests and modular rollouts, commands can be:
* **Officially supported native features** (like `/canvas`, keyboard shortcuts, and `@` Custom GPT mentions).
* **Experimental/Beta features** or flags (workspace and lab rollouts).
* **Semantic/Pseudo-commands** (user-defined shorthands powered by Custom Instructions or System Prompts that GPT models interpret natively with absolute precision).

This handbook details all three levels of commands to provide a complete, master-level reference for power users.

---

## Table of Contents

1. [Understanding ChatGPT Commands](#1-understanding-chatgpt-commands)
2. [Official Core Slash Commands](#2-official-core-slash-commands)
3. [Workspace & Canvas Commands](#3-workspace--canvas-commands)
4. [File & Document Commands](#4-file--document-commands)
5. [Image & Media Commands](#5-image--media-commands)
6. [Voice & Camera Commands](#6-voice--camera-commands)
7. [Memory & Search Commands](#7-memory--search-commands)
8. [Developer & Coding Commands](#8-developer--coding-commands)
9. [Analysis & Strategy Commands](#9-analysis--strategy-commands)
10. [Writing & Editing Commands](#10-writing--editing-commands)
11. [Business & Founder Commands](#11-business--founder-commands)
12. [Research & Learning Commands](#12-research--learning-commands)
13. [Productivity Commands](#13-productivity-commands)
14. [Roleplay & Persona Commands](#14-roleplay--persona-commands)
15. [Community Power Commands](#15-community-power-commands)
16. [Hidden / Experimental Commands](#16-hidden--experimental-commands)
17. [Keyboard Shortcuts](#17-keyboard-shortcuts)
18. [Building Your Own Command Framework](#18-building-your-own-command-framework)
19. [Advanced Prompt Chaining](#19-advanced-prompt-chaining)
20. [Final Notes](#20-final-notes)

---

## 1. Understanding ChatGPT Commands

To master commands in ChatGPT, you must first understand that they are processed at different layers of the application stack. Here is the operational breakdown:

| Type | Processed By | Meaning & Function | Example |
| :--- | :--- | :--- | :--- |
| **Official Commands** | ChatGPT UI / Core App | Hardcoded interface commands that trigger native application features, menus, navigation, or routing. | `/canvas` or `@` |
| **Contextual Commands** | Active Tools / Sandboxes | Commands enabled inside specific sandboxed interfaces, such as Canvas code editing or Python code interpreter environments. | `/comment` or `/update` |
| **Semantic Commands** | LLM Semantic Parser | Shorthand instructions interpreted natively by the LLM without requiring hardcoded UI components. | `/eli5` or `/tldr` |
| **Custom Commands** | System Prompts / Custom GPTs | Commands explicitly mapped by the user to multi-line instructions, APIs, or database queries. | User-defined `/audit` |

### Why use commands instead of natural language?
1. **Bandwidth Efficiency**: Reduces the volume of repetitive instruction tokens you need to write.
2. **Cognitive Routing**: Forces the LLM into a specific analytical mode (e.g., acting as a CTO vs. a copywriter).
3. **Structured Workflows**: Enables deterministic outputs from a single shorthand input.

> [!NOTE]
> When executing a command, the LLM parses the forward slash (`/`) as a semantic delimiter. In model training, slash syntax represents system-level or command-line parameters, making it highly effective for structured prompts.

---

## 2. Official Core Slash Commands

These are native UI commands, keyboard shortcuts, or platform routing tools built into the core ChatGPT interface (Web, Desktop, and Mobile).

### `/help`
* **Purpose**: Displays a list of application tips, tool instructions, or UI shortcuts.
* **Usage**: Type `/help` when you need to view active shortcuts, available Custom GPT integrations, or basic guidelines.
* **Example**:
  ```text
  /help
  ```

### `/new`
* **Purpose**: Instantly initializes a fresh, clean chat session.
* **Usage**: Perfect for starting a new topic without carrying over context tokens from your previous conversation.
* **Example**:
  ```text
  /new
  ```

### `/clear`
* **Purpose**: Empties the current session interface or wipes context history.
* **Usage**: Keeps the same chat thread open but clears the prompt history to prevent contextual bleed.
* **Example**:
  ```text
  /clear
  ```

### `/rename`
* **Purpose**: Renames the title of the current chat thread in the sidebar.
* **Usage**: Overrides the automatic title generation with a custom label of your choice.
* **Example**:
  ```text
  /rename AI Research Vault
  ```

### `/delete`
* **Purpose**: Permanently deletes the current active chat thread.
* **Usage**: Cleans up your history list immediately from within the prompt composer.
* **Example**:
  ```text
  /delete
  ```

### `/settings`
* **Purpose**: Opens the settings dialog or account preferences menu.
* **Usage**: Quickly modify voice settings, theme preferences, custom instructions, or model configurations.
* **Example**:
  ```text
  /settings
  ```

### `/about`
* **Purpose**: Displays system information, current model version, and platform status.
* **Usage**: Useful for verifying whether you are running the latest desktop update or checking experimental feature flags.
* **Example**:
  ```text
  /about
  ```

---

## 3. Workspace & Canvas Commands

These commands operate within **ChatGPT Canvas**, a side-by-side editing interface designed for writing and coding projects.

### `/canvas`
* **Purpose**: Manually launches a new collaborative Canvas window.
* **Usage**: If ChatGPT doesn't automatically trigger a Canvas for a long writing or coding project, use this command to force open the editor.
* **Example**:
  ```text
  /canvas build a scalable TypeScript SaaS boilerplate
  ```

### `/update`
* **Purpose**: Directs the editor to perform a major revision on the entire active document in the Canvas window.
* **Usage**: Apply universal changes such as programming language porting, style alterations, or global formatting updates.
* **Example**:
  ```text
  /update rewrite all examples in TypeScript using ESModules
  ```

### `/comment`
* **Purpose**: Analyzes the canvas content and adds inline comments, explanations, or code documentation.
* **Usage**: Highlights lines that need clarification or creates documentation strings for APIs.
* **Example**:
  ```text
  /comment add complete inline JSDoc comments to this class
  ```

### `/export`
* **Purpose**: Converts the current Canvas document into a downloadable file.
* **Usage**: Export files in formats like Markdown, HTML, PDF, or DOCX.
* **Example**:
  ```text
  /export markdown
  ```

---

## 4. File & Document Commands

These commands manage document parsing, data extraction, and semantic transformations.

### `/upload`
* **Purpose**: Prepares a file (PDF, CSV, TXT, DOCX, etc.) to be uploaded and parsed into the active context window.
* **Usage**: Reference a file by name to instruct the document analyzer to index it.
* **Example**:
  ```text
  /upload investor_pitch_deck_v4.pdf
  ```

### `/analyze`
* **Purpose**: Triggers the Advanced Data Analysis sandbox (Python) to read, clean, and run statistics on uploaded datasets.
* **Usage**: Use on structured files (CSV, JSON, XLSX) to generate statistics, correlations, or mathematical reports.
* **Example**:
  ```text
  /analyze quarterly_revenue.csv
  ```

### `/summarize`
* **Purpose**: Compresses long documents, logs, or books into digestible bullet points or executive summaries.
* **Usage**: Specify target length, format, or focus areas.
* **Example**:
  ```text
  /summarize this document in 5 key executive bullet points focusing on financial risks
  ```

### `/translate`
* **Purpose**: Translates the specified document or block of text into another language while maintaining tone.
* **Usage**: State the target language and any cultural localization preferences.
* **Example**:
  ```text
  /translate English to Japanese using formal business honorifics (Keigo)
  ```

### `/extract`
* **Purpose**: Scans a large text block to retrieve specific data points (dates, names, values, actions).
* **Usage**: Excellent for parsing raw emails, meeting transcripts, or legal contracts.
* **Example**:
  ```text
  /extract all actionable items, owners, and deadlines from this meeting transcript
  ```

### `/ocr`
* **Purpose**: Performs Optical Character Recognition on an uploaded image, scanned PDF, or screenshot.
* **Usage**: Extract text from hand-written notes, receipts, whiteboard diagrams, or code screenshots.
* **Example**:
  ```text
  /ocr extract the text and calculate the total sum from this receipt image
  ```

---

## 5. Image & Media Commands

These commands control DALL-E image generation, visual editing, and chart rendering.

### `/image`
* **Purpose**: Triggers DALL-E to generate a visual asset from a detailed descriptive prompt.
* **Usage**: Provide details on lighting, camera angle, style, color palette, and subject.
* **Example**:
  ```text
  /image cinematic 35mm photograph of a futuristic cyberpunk Kolkata skyline during a heavy monsoon night, neon sign reflections on wet streets
  ```

### `/edit-image`
* **Purpose**: Instructs the model to perform target modifications on an existing or generated image.
* **Usage**: Define the changes relative to the original image (e.g., adding/removing objects, altering colors).
* **Example**:
  ```text
  /edit-image change the background from daytime to a starry night and add a crescent moon
  ```

### `/describe-image`
* **Purpose**: Analyzes the contents, composition, color palette, and typography of an uploaded image.
* **Usage**: Use for alt-text generation, reverse engineering image prompts, or design reviews.
* **Example**:
  ```text
  /describe-image explain the design layout and font choices of this landing page screenshot
  ```

### `/make-chart`
* **Purpose**: Generates interactive charts, graphs, or heatmaps from data tables.
* **Usage**: Uses Python (Matplotlib/Seaborn) or Mermaid.js to build visual data representations.
* **Example**:
  ```text
  /make-chart startup revenue growth projection for the next 5 years based on the uploaded CSV
  ```

### `/diagram`
* **Purpose**: Renders diagrams, architectural system graphs, or flowcharts.
* **Usage**: Generates charts using Mermaid syntax or visual libraries.
* **Example**:
  ```text
  /diagram microservice authentication flow with OAuth2 and JWT tokens
  ```

### `/mockup`
* **Purpose**: Generates a high-fidelity visual UI/UX layout concept.
* **Usage**: Describe the user interface layout, platform (Mobile/Web), and color scheme.
* **Example**:
  ```text
  /mockup dashboard UI for a B2B SaaS analytics tool, dark mode, glassmorphic UI elements
  ```

---

## 6. Voice & Camera Commands

These commands are used on mobile and desktop apps with audio/video hardware integrations.

### `/voice`
* **Purpose**: Activates the real-time audio interaction channel.
* **Usage**: Initiate hands-free conversations with human-like latency.
* **Example**:
  ```text
  /voice
  ```

### `/listen`
* **Purpose**: Sets the microphone to continuous transcription mode.
* **Usage**: Ideal for dictation, transcribing live meetings, or brainstorming aloud.
* **Example**:
  ```text
  /listen
  ```

### `/camera`
* **Purpose**: Requests access to the camera to take a photo or scan a physical environment.
* **Usage**: Analyze physical objects, read error messages on monitors, or solve math problems on paper.
* **Example**:
  ```text
  /camera
  ```

---

## 7. Memory & Search Commands

These commands manage ChatGPT's persistent memory and database queries.

### `/memory`
* **Purpose**: Queries, updates, or audits the facts the model has stored about you across chat sessions.
* **Usage**: View saved profile data, delete outdated preferences, or manually add a new fact.
* **Example**:
  ```text
  /memory what do you know about my tech stack preferences?
  ```

### `/search`
* **Purpose**: Performs a semantic search across your entire chat history.
* **Usage**: Retrieve past explanations, code snippets, or notes without manual scrolling.
* **Example**:
  ```text
  /search Docker deployment configuration for Node.js
  ```

### `/tools`
* **Purpose**: Lists all APIs, plug-ins, and extensions available in the current workspace.
* **Usage**: Identify available tool parameters and sandbox runtimes.
* **Example**:
  ```text
  /tools
  ```

### `/model`
* **Purpose**: Explicitly switches the current reasoning engine or references model characteristics.
* **Usage**: Direct the system to run on a specialized model version (e.g., standard vs. reasoning models).
* **Example**:
  ```text
  /model GPT-5.5
  ```

---

## 8. Developer & Coding Commands

These commands streamline software development, debugging, and systems engineering.

### `/debug`
* **Purpose**: Enters deep diagnostic mode to trace errors, stack traces, and logic flaws.
* **Usage**: Provide the error message, target environment, and broken code.
* **Example**:
  ```text
  /debug React hydration mismatch error when loading next-themes wrapper
  ```

### `/refactor`
* **Purpose**: Optimizes code structure, design patterns, and readability without modifying external behavior.
* **Usage**: Specify target design patterns, modularity goals, or language standards.
* **Example**:
  ```text
  /refactor this legacy vanilla JavaScript file into modular ES6 modules using functional patterns
  ```

### `/optimize`
* **Purpose**: Optimizes algorithms, database queries, and system architectures for performance and memory.
* **Usage**: Focus on asymptotic complexity (Big O), indexing, caching, or load reduction.
* **Example**:
  ```text
  /optimize this PostgreSQL query that joins multiple high-volume log tables
  ```

### `/review`
* **Purpose**: Conducts a security and code quality review.
* **Usage**: Identifies potential security bugs (SQL Injection, XSS) and anti-patterns.
* **Example**:
  ```text
  /review check this custom Node.js authentication middleware for security vulnerabilities
  ```

### `/explain`
* **Purpose**: Breaks down complex source code, packages, or architectural styles.
* **Usage**: Great for onboarding to unfamiliar codebases or learning new systems.
* **Example**:
  ```text
  /explain how this Redis pub/sub queue implements backpressure handling
  ```

### `/generate-tests`
* **Purpose**: Writes unit, integration, or end-to-end tests.
* **Usage**: State the testing library and specific edge cases to cover.
* **Example**:
  ```text
  /generate-tests using Jest and React Testing Library for this user profile form component
  ```

### `/document`
* **Purpose**: Generates JSDoc, Docstrings, OpenAPI/Swagger specifications, or README files.
* **Usage**: Feed raw classes or APIs to generate clear, structured documentation.
* **Example**:
  ```text
  /document write a complete README.md and OpenAPI 3.0 spec for this Express router file
  ```

---

## 9. Analysis & Strategy Commands

These commands assist with business model validation, strategic planning, and risk mitigation.

### `/critique`
* **Purpose**: Critically evaluates startup pitch decks, product designs, or marketing plans.
* **Usage**: Instructs the model to adopt a analytical, critical persona to find flaws.
* **Example**:
  ```text
  /critique this landing page layout and copy like a cynical Y Combinator partner
  ```

### `/actionplan`
* **Purpose**: Translates high-level goals into granular, step-by-step task lists.
* **Usage**: Outline resources, milestones, dependencies, and timelines.
* **Example**:
  ```text
  /actionplan launch a cold email outreach system for an AI automation agency in 30 days
  ```

### `/roadmap`
* **Purpose**: Generates long-term operational and product development timelines.
* **Usage**: Map milestones across months or quarters.
* **Example**:
  ```text
  /roadmap transition from monolithic infrastructure to a microservices architecture over 12 months
  ```

### `/strategy`
* **Purpose**: Formulates growth, monetization, distribution, or positioning tactics.
* **Usage**: Analyze competitors, target audiences, and market dynamics.
* **Example**:
  ```text
  /strategy organic acquisition channels for a B2B SaaS targeting mid-market marketing heads
  ```

### `/framework`
* **Purpose**: Creates reusable mental models or operational frameworks.
* **Usage**: Standardize operations, content production, or hiring processes.
* **Example**:
  ```text
  /framework dynamic pricing model for an API-first database startup
  ```

### `/decision`
* **Purpose**: Analyzes trade-offs, opportunity costs, and strategic routes.
* **Usage**: Compare paths (e.g., Bootstrapping vs. VC funding).
* **Example**:
  ```text
  /decision bootstrap vs. seed funding round for a developer tools company
  ```

### `/risk-analysis`
* **Purpose**: Conducts failure-mode analysis on system rollouts or business operations.
* **Usage**: Identify security, operational, legal, and financial risk vectors.
* **Example**:
  ```text
  /risk-analysis implementing decentralized crypto payment gateways in a traditional e-commerce app
  ```

---

## 10. Writing & Editing Commands

These commands handle creative writing, content editing, and layout outlining.

### `/rewrite`
* **Purpose**: Alters the tone, format, style, or reading level of a text.
* **Usage**: Keep original meaning but adjust style.
* **Example**:
  ```text
  /rewrite this copy to sound like a premium, sleek luxury fintech brand targeting Gen Z
  ```

### `/shorten`
* **Purpose**: Compresses sentences without losing key information.
* **Usage**: Ideal for editing tweets, ads, or email subject lines.
* **Example**:
  ```text
  /shorten this cold outreach email to fit on a single mobile screen (under 120 words)
  ```

### `/expand`
* **Purpose**: Elaborates on short concepts with additional details and context.
* **Usage**: Expand notes, draft outlines, or add detail to short paragraphs.
* **Example**:
  ```text
  /expand this rough outline into a detailed introductory chapter for a book on prompt engineering
  ```

### `/outline`
* **Purpose**: Builds a logical structure for books, essays, courses, or presentations.
* **Usage**: Organize headings, subheadings, and key points.
* **Example**:
  ```text
  /outline a 10-part masterclass syllabus on AI agents and autonomous workflows
  ```

### `/brainstorm`
* **Purpose**: Generates creative ideas, slogans, angles, or titles.
* **Usage**: Provide details on the target market, goals, and style guidelines.
* **Example**:
  ```text
  /brainstorm 15 unique hook angles for a SaaS targeting email marketing managers
  ```

### `/hooks`
* **Purpose**: Writes high-converting hooks for social media, ads, or copy.
* **Usage**: Focus on curiosity, pain points, or statistics.
* **Example**:
  ```text
  /hooks for a short video explaining how AI models parse programming languages
  ```

### `/caption`
* **Purpose**: Drafts short captions optimized for specific social networks.
* **Usage**: Mention platforms (LinkedIn, Instagram) and include relevant emojis or hashtags.
* **Example**:
  ```text
  /caption LinkedIn post detailing our new dev tool update, keeping it developer-focused
  ```

### `/thread`
* **Purpose**: Formats long stories or insights into Twitter/X threads.
* **Usage**: Break down text into numbered posts with hook leads.
* **Example**:
  ```text
  /thread explaining how the Transformers architecture changed modern computing
  ```

### `/script`
* **Purpose**: Drafts visual and spoken scripts for video content.
* **Usage**: Outline visual directions, sound effects, and spoken dialogue.
* **Example**:
  ```text
  /script a 90-second YouTube Short explaining database indexing to junior developers
  ```

### `/tldr`
* **Purpose**: Generates a quick, single-sentence summary of long text.
* **Usage**: Create concise summaries of articles, briefs, or logs.
* **Example**:
  ```text
  /tldr summarize the attached 40-page whitepaper on AI safety regulations
  ```

### `/eli5`
* **Purpose**: Translates complex technical topics into simple, relatable analogies.
* **Usage**: Explain advanced engineering or scientific concepts to a general audience.
* **Example**:
  ```text
  /eli5 how zero-knowledge proofs work without using mathematical formulas
  ```

---

## 11. Business & Founder Commands

These commands model executive roles and support operational tasks for startup founders.

### `/founder`
* **Purpose**: Triggers a strategic executive coaching mode.
* **Usage**: Validate product-market fit, draft investor updates, or design company culture.
* **Example**:
  ```text
  /founder validate this hypothesis: developers will pay for an AI-powered git hook manager
  ```

### `/cto`
* **Purpose**: Acts as a seasoned Chief Technology Officer.
* **Usage**: Select tech stacks, design systems architectures, and evaluate security practices.
* **Example**:
  ```text
  /cto design a high-throughput, low-latency API architecture for a real-time multiplayer game
  ```

### `/cmo`
* **Purpose**: Acts as a growth marketing executive.
* **Usage**: Map out growth loops, user acquisition channels, and viral loops.
* **Example**:
  ```text
  /cmo design a low-budget, organic growth strategy to acquire the first 1,000 developer users
  ```

### `/sales`
* **Purpose**: Refines sales scripts, objection-handling scripts, and closing frameworks.
* **Usage**: Prepare for sales calls or negotiate contracts.
* **Example**:
  ```text
  /sales write an objection-handling matrix for: "your developer tool is too expensive compared to self-hosting"
  ```

### `/offer`
* **Purpose**: Packages services or software tiers into high-value offers.
* **Usage**: Map pricing tiers, value props, and bonuses.
* **Example**:
  ```text
  /offer package our cloud migration consulting service into three distinct retainer options
  ```

### `/funnel`
* **Purpose**: Diagrams and plans conversion paths for user acquisition.
* **Usage**: Design user journeys from initial touchpoint to purchase.
* **Example**:
  ```text
  /funnel map out the user conversion path for a freemium developer tool
  ```

### `/proposal`
* **Purpose**: Writes high-converting business or technical consulting proposals.
* **Usage**: Outline project scopes, deliverables, timelines, and costs.
* **Example**:
  ```text
  /proposal write a custom proposal for migrating a legacy PHP app to a serverless architecture
  ```

### `/coldemail`
* **Purpose**: Drafts personalized cold outreach emails.
* **Usage**: Personalize hooks, value propositions, call-to-actions, and follow-ups.
* **Example**:
  ```text
  /coldemail reach out to VP of Engineering leads offering custom security audit automation
  ```

---

## 12. Research & Learning Commands

These commands support deep academic research, structured learning, and concept comparisons.

### `/research`
* **Purpose**: Triggers an academic research workflow.
* **Usage**: Synthesize scientific literature, cite research sources, and evaluate methodologies.
* **Example**:
  ```text
  /research the evolution of retrieval-augmented generation (RAG) techniques from 2020 to 2026
  ```

### `/compare`
* **Purpose**: Generates detailed comparison matrices across multiple dimensions.
* **Usage**: Evaluate technologies, frameworks, strategies, or competitors.
* **Example**:
  ```text
  /compare Rust vs. Go for microservices handling real-time WebSockets
  ```

### `/proscons`
* **Purpose**: Lists pros, cons, tradeoffs, and risks for a given decision.
* **Usage**: Weigh architectural patterns or business configurations.
* **Example**:
  ```text
  /proscons using a managed database service vs. self-hosting on raw EC2 instances
  ```

### `/step-by-step`
* **Purpose**: Breaks complex logical tasks into sequential reasoning chains.
* **Usage**: Solves math, physics, logic, or complex troubleshooting tasks step-by-step.
* **Example**:
  ```text
  /step-by-step calculate the network latency overhead of adding mutual TLS (mTLS) to this cluster
  ```

### `/quiz`
* **Purpose**: Generates interactive test questions to test retention.
* **Usage**: Assess knowledge on a topic with multiple choice or open-ended questions.
* **Example**:
  ```text
  /quiz generate a 5-question test on Kubernetes networking and Pod IP routing
  ```

### `/studyplan`
* **Purpose**: Curates a complete self-directed syllabus and schedule.
* **Usage**: Structure learning journeys with curated topics, resources, and timelines.
  ```text
  /studyplan build a 12-week curriculum to transition from Python beginner to machine learning engineer
  ```

---

## 13. Productivity Commands

These commands convert raw ideas into structured productivity tools.

### `/checklist`
* **Purpose**: Turns a project plan or goal into a detailed, operational checklist.
* **Usage**: Ensure operational accuracy during complex deployments or onboarding.
* **Example**:
  ```text
  /checklist pre-launch deployment check list for a production web application
  ```

### `/todo`
* **Purpose**: Creates an action-item checklist based on recent chat notes.
* **Usage**: Translate notes into immediate daily tasks.
  ```text
  /todo summarize our chat notes on SEO optimization into a prioritized checklist
  ```

### `/calendar`
* **Purpose**: Creates structured content, training, or project calendars.
* **Usage**: Map out daily or weekly tasks over time.
  ```text
  /calendar design a 30-day posting schedule for developer-facing tech tutorials
  ```

### `/prioritize`
* **Purpose**: Evaluates task lists and ranks them using frameworks like the Eisenhower Matrix.
* **Usage**: Focus on high-leverage tasks.
  ```text
  /prioritize evaluate these 12 startup tasks by urgency, impact, and effort required
  ```

### `/automation`
* **Purpose**: Designs workflow blueprints using tools like Zapier, n8n, or Make.com.
* **Usage**: Standardize lead routing, file conversions, or database synchronization.
  ```text
  /automation design a workflow to parse incoming PDFs, run sentiment analysis, and alert Slack
  ```

---

## 14. Roleplay & Persona Commands

These commands simulate environments and personas for training, practice, or analysis.

### `/act-as`
* **Purpose**: Assigns a highly specialized persona to the model.
* **Usage**: Adopt specific expertise (e.g., UI designer, security auditor, recruiter).
* **Example**:
  ```text
  /act-as an expert cybersecurity auditor specialized in parsing AWS IAM configurations
  ```

### `/simulate`
* **Purpose**: Creates interactive, branch-based simulations.
* **Usage**: Roleplay presentations, crisis management scenarios, or negotiations.
* **Example**:
  ```text
  /simulate an interactive investor meeting where I pitch my startup and you raise objections
  ```

### `/debate`
* **Purpose**: Explores and defends competing viewpoints on a controversial topic.
* **Usage**: Uncover bias, test assumptions, or understand opposing arguments.
* **Example**:
  ```text
  /debate argue both sides of the remote-first vs. hybrid workspace model
  ```

### `/interview`
* **Purpose**: Conducts a mock job interview.
* **Usage**: Practice technical or behavioral questions with real-time feedback.
* **Example**:
  ```text
  /interview me for a Senior Go Backend Engineer role, asking one question at a time
  ```

---

## 15. Community Power Commands

These commands are developed by AI community power users to push LLM reasoning limits.

### `/deepdive`
* **Purpose**: Triggers a thorough, multi-layered research analysis.
* **Usage**: Skip superficial summaries to analyze root causes, histories, and mechanics.
* **Example**:
  ```text
  /deepdive the history and technical limitations of the WebAssembly ecosystem
  ```

### `/mentalmodel`
* **Purpose**: Explains concepts using established mental models (e.g., Pareto Principle, Inversion).
* **Usage**: Approach business or technical problems from different analytical angles.
* **Example**:
  ```text
  /mentalmodel explain startup customer retention using Second-Order Thinking
  ```

### `/firstprinciples`
* **Purpose**: Deconstructs assumptions down to fundamental truth vectors.
* **Usage**: Solve complex problems by rebuilding solutions from the ground up.
* **Example**:
  ```text
  /firstprinciples how can we lower server cost without reducing response speed
  ```

### `/simplify`
* **Purpose**: Removes jargon and simplifies complex text.
* **Usage**: Make academic papers or technical documentation accessible.
* **Example**:
  ```text
  /simplify this complex research paper on quantum error correction codes
  ```

### `/roast`
* **Purpose**: Points out design flaws, writing weaknesses, or business risks using humor.
* **Usage**: A fun, critical audit of designs, copy, or strategies.
* **Example**:
  ```text
  /roast my portfolio landing page and layout copy
  ```

### `/improve`
* **Purpose**: Analyzes text and recommends three specific improvement routes.
* **Usage**: Refine copy, optimize code quality, or polish marketing text.
* **Example**:
  ```text
  /improve this user registration email sequence to boost open rates
  ```

### `/nextsteps`
* **Purpose**: Generates immediate action steps for the next 24 to 72 hours.
* **Usage**: Avoid analysis paralysis by identifying immediate priorities.
* **Example**:
  ```text
  /nextsteps we just launched our project, how do we begin gathering user feedback?
  ```

---

## 16. Hidden / Experimental Commands

These commands are associated with internal workspace rollouts, feature flags, or model routing.

### `/gpts`
* **Purpose**: Displays the Custom GPT selection menu.
* **Usage**: Choose from specialized, community-built GPT configurations.
* **Example**:
  ```text
  /gpts
  ```

### `/agents`
* **Purpose**: Triggers autonomous multi-step loops or agentic tools.
* **Usage**: Set multi-step goals that run in the background.
* **Example**:
  ```text
  /agents scrape the latest tech headlines and email me a formatted summary
  ```

### `/tasks`
* **Purpose**: Interacts with background execution loops or scheduled prompts.
* **Usage**: Manage, cancel, or edit active agent runs.
* **Example**:
  ```text
  /tasks list
  ```

### `/browse`
* **Purpose**: Forces ChatGPT to search the web using Bing.
* **Usage**: Ensure the model uses real-time search instead of its pre-trained knowledge base.
* **Example**:
  ```text
  /browse search for the latest regulatory updates on AI compliance passed this week
  ```

### `/plugins`
* **Purpose**: Accesses legacy external integration configurations.
* **Usage**: Connect with third-party web apps (e.g., WolframAlpha, Zapier).
* **Example**:
  ```text
  /plugins
  ```

### `/code`
* **Purpose**: Puts the editor in code-only mode.
* **Usage**: Minimizes conversational text to focus on clean code blocks.
* **Example**:
  ```text
  /code write a clean implementation of the A* search algorithm in Rust
  ```

### `/python`
* **Purpose**: Triggers the interactive Python interpreter sandboxed environment.
* **Usage**: Run calculations, plot graphs, or manipulate datasets in real time.
* **Example**:
  ```text
  /python calculate the prime factors of 9837428974 and plot their distribution
  ```

---

## 17. Keyboard Shortcuts

Using keyboard shortcuts alongside slash commands helps you navigate ChatGPT efficiently without touching your mouse.

| Action | Windows / Linux | macOS |
| :--- | :--- | :--- |
| **New Chat** | `Ctrl` + `Shift` + `O` | `Cmd` + `Shift` + `O` |
| **Search Chats** | `Ctrl` + `K` | `Cmd` + `K` |
| **Toggle Sidebar** | `Ctrl` + `Shift` + `S` | `Cmd` + `Shift` + `S` |
| **Show All Shortcuts** | `Ctrl` + `/` | `Cmd` + `/` |
| **Copy Last Response** | `Ctrl` + `Shift` + `C` | `Cmd` + `Shift` + `C` |
| **Copy Last Code Block** | `Ctrl` + `Shift` + `;` | `Cmd` + `Shift` + `;` |
| **New Line (in composer)**| `Shift` + `Enter` | `Shift` + `Enter` |
| **Quick Launch App** | `Alt` + `Space` | `Option` + `Space` |

---

## 18. Building Your Own Command Framework

You don't have to wait for OpenAI to release official slash commands. You can build your own command system using **Custom Instructions** or by creating a **Custom GPT**.

### The Custom Command Blueprint (System Prompt Template)

Copy and paste this system prompt into the **"How would you like ChatGPT to respond?"** section of your Custom Instructions, or into the **Instructions** panel of a Custom GPT:

```text
You are an advanced, high-performance command-driven AI operating system. 
You must recognize and execute the following slash commands immediately. 
If the user's message starts with a slash command, bypass default conversational responses and execute the instructions mapped to that command:

[COMMAND DICTIONARY]
- /eli5: Explain the input concept using simple analogies, bypassing technical jargon entirely. Format for a 10-year-old child.
- /cto: Analyze the input query from a systems architect perspective. Provide structural diagrams (Mermaid.js), select optimal frameworks, and identify performance bottlenecks.
- /critique: Act as a ruthless startup advisor. Audit the input content, list exactly 5 critical flaws, and offer actionable fixes for each.
- /refactor: Reorganize the input code to follow modular, clean-code practices, JSDoc conventions, and optimal Big-O performance. Print the refactored code block and a quick bulleted list of changes.
- /tldr: Provide a single-sentence summary of the input text under 20 words, followed by exactly three bullet points of key takeaways.
- /actionplan: Create a detailed, prioritized implementation checklist from the input goals, including timelines, milestones, and potential risk factors.

[EXECUTION PROTOCOL]
- If a command is triggered, start the response with: "⚡ [Command Name] Mode Activated" on the first line.
- Present outputs with clean markdown headings, bold accents, and code block formatting where appropriate.
```

---

## 19. Advanced Prompt Chaining

Once your command framework is set up, you can chain multiple commands in a single prompt to build complex, automated workflows.

### Workflow 1: The Founder's Strategic Suite
* **Goal**: Research a market, critique the strategy, and write a roadmap.
* **Chained Prompt**:
  ```text
  /research the growing market of self-hosted open-source monitoring databases.
  ---
  /critique our strategy of targeting enterprise teams with a $49/month tier.
  ---
  /roadmap draft our 6-month product development and marketing roadmap.
  ```

### Workflow 2: The Code Polish Line
* **Goal**: Explain, refactor, and write tests for a legacy file.
* **Chained Prompt**:
  ```text
  /explain this complex file: [Insert Code]
  ---
  /refactor into clean TypeScript using functional patterns.
  ---
  /generate-tests using Jest to cover all edge cases.
  ```

### Workflow 3: The Content Creation Engine
* **Goal**: Brainstorm startup ideas, write hooks, and generate scripts.
* **Chained Prompt**:
  ```text
  /brainstorm 5 startup ideas solving cloud billing challenges.
  ---
  /hooks create high-converting marketing hooks for the winning idea.
  ---
  /script write a 60-second video script explaining the tool's core value proposition.
  ```

---

## 20. Final Notes

Slash commands are more than simple shortcuts—they are:
* **Cognitive Routing Systems**: They steer the LLM's neural network into specialized reasoning states.
* **Modular Workflows**: They bundle complex, multi-step instructions into single triggers.
* **Actionable Intent Compilers**: They convert vague natural language into structured, predictable formats.

By implementing custom command frameworks, you transition from basic chatting to building personal, command-driven AI applications.

*Built for operators running at terminal velocity.* ⚡

<br />

<p align="center">
  <a href="https://linktr.ee/YourAKShaw" target="_blank">
    <img src="https://i.ibb.co/WWtQx1vW/Your-AKShaw-follow-me-v1-rounded-corners-reduce-size-modified.png" alt="Follow AK Shaw on Linktree" width="400" />
  </a>
</p>