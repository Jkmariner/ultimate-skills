# Ultimate Agent Skills

A portable library of **72 reusable agent skills** for **Hermes**, **Antigravity**, and **Claude Code**. Browse the catalog below, install the skills you need, and invoke them by name or let your agent select them when relevant.

**[Latest release: v1.1.0](https://github.com/Jkmariner/ultimate-skills/releases/tag/v1.1.0)** · **[MIT License](./LICENSE)**

> These are instruction packs for your existing agent, not separate AI models or agents. What an agent can do still depends on its model, tools, permissions, and the context you provide. A skill does not grant additional access or permissions.

## Contents

- [What is an agent skill?](#what-is-an-agent-skill)
- [Quick start](#quick-start)
- [Skill catalog](#skill-catalog)
- [Install for Hermes, Antigravity, or Claude Code](#install-for-hermes-antigravity-or-claude-code)
- [How to use a skill](#how-to-use-a-skill)
- [Update, troubleshoot, and validate](#update-troubleshoot-and-validate)
- [License](#license)

## What is an agent skill?

A skill is a focused set of instructions that teaches an agent how to approach a recurring task. Each skill lives in its own folder and has a `SKILL.md` file containing a name, a description that helps the agent recognize when to use it, a workflow, and task-specific guidance.

Skills use the shared [Agent Skills format](https://agentskills.io/specification). They are designed to work across agent platforms, but each platform has its own installation locations and may expose skills differently. Skills do not include or install models, tools, APIs, or external services. In particular, installing the same skill on multiple platforms does not connect those platforms to one another; cross-agent delegation requires orchestration support from the platform or an external integration.

## Quick start

1. Browse the [skill catalog](#skill-catalog) and choose a skill folder.
2. Install that folder into the supported skills directory for your agent (see [installation instructions](#install-for-hermes-antigravity-or-claude-code)).
3. Start a new agent session if the skill is not detected.
4. Ask for the task naturally or invoke the skill by its slash command, for example:

   ```text
   /study-group-facilitator Plan a 60-minute review session for our biology exam.
   ```

For work that benefits from several perspectives, install and invoke **Adaptive Agent Team**. It delegates to separate subagents only when your platform provides that capability; otherwise, the current agent switches roles internally and is clear that it is doing so.

### At a glance

| Area | Skills |
|---|---:|
| Core assistance | 9 |
| Software and technology | 12 |
| Research, writing, and learning | 9 |
| Education, school, and college | 17 |
| Data, analysis, and operations | 9 |
| Product, design, and business | 10 |
| Personal and specialist support | 6 |
| **Total** | **72** |

## Skill catalog

## Core skills

| Skill | What it helps with |
|---|---|
| [Task Planner](./skills/task-planner/SKILL.md) | Turn a goal into a clear, prioritized plan with assumptions and checkpoints. |
| [General Researcher](./skills/general-researcher/SKILL.md) | Find, compare, and summarize reliable information with sources. |
| [File and Document Assistant](./skills/file-and-document-assistant/SKILL.md) | Read, organize, transform, and draft common documents and files. |
| [Clear Communication](./skills/clear-communication/SKILL.md) | Adapt explanations, emails, and messages to the audience and tone. |
| [Decision Support](./skills/decision-support/SKILL.md) | Compare options against explicit criteria and explain trade-offs. |
| [Workflow Automator](./skills/workflow-automator/SKILL.md) | Identify repetitive steps and automate them safely with available tools. |
| [Quality Checker](./skills/quality-checker/SKILL.md) | Review work against a checklist, requirements, and acceptance criteria. |
| [Knowledge Organizer](./skills/knowledge-organizer/SKILL.md) | Turn notes and scattered material into structured, searchable knowledge. |
| [Adaptive Agent Team](./skills/adaptive-agent-team/SKILL.md) | Coordinate specialist roles, delegate independent work when supported, and synthesize a checked result. |

## Software and technology

| Skill | What it helps with |
|---|---|
| [Software Builder](./skills/software-builder/SKILL.md) | Implement scoped features while following the repository's existing patterns. |
| [Code Explainer](./skills/code-explainer/SKILL.md) | Explain code, architecture, APIs, and data flow at the requested level. |
| [Debugging Assistant](./skills/debugging-assistant/SKILL.md) | Reproduce and isolate failures, inspect evidence, and verify a fix. |
| [Code Reviewer](./skills/code-reviewer/SKILL.md) | Find correctness, maintainability, and regression risks in a proposed change. |
| [Test Engineer](./skills/test-engineer/SKILL.md) | Design and run focused tests for stated behavior and edge cases. |
| [Refactoring Assistant](./skills/refactoring-assistant/SKILL.md) | Improve structure without intentionally changing observable behavior. |
| [Documentation Writer](./skills/documentation-writer/SKILL.md) | Create or update user, developer, and API documentation. |
| [API and Integration Builder](./skills/api-and-integration-builder/SKILL.md) | Design and connect services, APIs, webhooks, and data contracts. |
| [Database Assistant](./skills/database-assistant/SKILL.md) | Help with schemas, queries, migrations, and data modeling. |
| [DevOps Assistant](./skills/devops-assistant/SKILL.md) | Help with builds, CI/CD, containers, deployments, and infrastructure configuration. |
| [Accessibility Checker](./skills/accessibility-checker/SKILL.md) | Review interfaces and content for accessibility issues and improvements. |
| [Localization Assistant](./skills/localization-assistant/SKILL.md) | Prepare interfaces and content for translation and regional conventions. |

## Research, writing, and learning

| Skill | What it helps with |
|---|---|
| [Technical Researcher](./skills/technical-researcher/SKILL.md) | Investigate technical questions and produce evidence-based summaries. |
| [Market Researcher](./skills/market-researcher/SKILL.md) | Compare markets, products, competitors, and customer needs from available sources. |
| [Source and Fact Checker](./skills/source-and-fact-checker/SKILL.md) | Verify claims, dates, quotations, and citations; flag uncertainty. |
| [Report Writer](./skills/report-writer/SKILL.md) | Produce structured briefs, reports, proposals, and executive summaries. |
| [Editor and Proofreader](./skills/editor-and-proofreader/SKILL.md) | Improve clarity, grammar, structure, and consistency while preserving intent. |
| [Presentation Builder](./skills/presentation-builder/SKILL.md) | Create an outline and speaker-ready content for presentations. |
| [Tutor and Study Coach](./skills/tutor-and-study-coach/SKILL.md) | Explain concepts, create practice questions, and adapt to the learner. |
| [Curriculum Designer](./skills/curriculum-designer/SKILL.md) | Organize learning goals into lessons, activities, and assessments. |
| [Translator](./skills/translator/SKILL.md) | Translate user-provided content while preserving meaning, tone, and terminology. |

## Education, school, and college

| Skill | What it helps with |
|---|---|
| [Student Study Coach](./skills/student-study-coach/SKILL.md) | Build realistic study plans, routines, and review schedules for school or college courses. |
| [Subject Tutor](./skills/subject-tutor/SKILL.md) | Explain school and college concepts step by step, adapting examples to the learner's level. |
| [Homework Guide](./skills/homework-guide/SKILL.md) | Help students understand prompts, break problems into steps, and learn the method rather than simply supplying answers. |
| [Exam and Quiz Prep](./skills/exam-and-quiz-prep/SKILL.md) | Create practice questions, review plans, flashcards, and mock quizzes from supplied course material. |
| [Notes and Lecture Organizer](./skills/notes-and-lecture-organizer/SKILL.md) | Turn a student's notes or lecture transcripts into organized summaries, key terms, and review prompts. |
| [Math Problem Coach](./skills/math-problem-coach/SKILL.md) | Explain mathematical reasoning and guide students through problems with checks for understanding. |
| [Science Learning Assistant](./skills/science-learning-assistant/SKILL.md) | Explain science concepts, help interpret class materials, and support safe, classroom-appropriate lab preparation. |
| [Reading Comprehension Coach](./skills/reading-comprehension-coach/SKILL.md) | Help analyze assigned readings, identify themes, and practice comprehension strategies. |
| [Academic Writing Coach](./skills/academic-writing-coach/SKILL.md) | Help plan, structure, revise, and cite student writing while preserving the student's own ideas and voice. |
| [Research and Citation Coach](./skills/research-and-citation-coach/SKILL.md) | Help students narrow a research question, evaluate sources, and format citations using the requested style. |
| [Language Learning Coach](./skills/language-learning-coach/SKILL.md) | Practice vocabulary, grammar, reading, and conversation at the learner's level. |
| [College Application Organizer](./skills/college-application-organizer/SKILL.md) | Track application requirements, deadlines, essays, and recommendation requests; help brainstorm without misrepresenting the student. |
| [College and Career Planner](./skills/college-and-career-planner/SKILL.md) | Compare programs and career paths against a student's interests, goals, and constraints. |
| [Financial Aid and Scholarship Organizer](./skills/financial-aid-and-scholarship-organizer/SKILL.md) | Organize deadlines and explain application instructions; direct students to official sources for eligibility and award details. |
| [Student Time and Assignment Planner](./skills/student-time-and-assignment-planner/SKILL.md) | Break down syllabi and assignment dates into manageable tasks and reminders. |
| [Study Group Facilitator](./skills/study-group-facilitator/SKILL.md) | Create agendas, discussion questions, and collaborative review activities for student groups. |
| [Student Accessibility Support](./skills/student-accessibility-support/SKILL.md) | Help organize accommodation requests and accessible study strategies; defer formal eligibility decisions to the school or college. |

## Data, analysis, and operations

| Skill | What it helps with |
|---|---|
| [Spreadsheet Analyst](./skills/spreadsheet-analyst/SKILL.md) | Clean, analyze, summarize, and explain spreadsheet data. |
| [Data Analyst](./skills/data-analyst/SKILL.md) | Explore datasets, calculate metrics, identify patterns, and communicate caveats. |
| [Data Visualization Assistant](./skills/data-visualization-assistant/SKILL.md) | Select and explain charts that match the data and question. |
| [SQL Assistant](./skills/sql-assistant/SKILL.md) | Draft, explain, and review SQL queries and database results. |
| [Process Mapper](./skills/process-mapper/SKILL.md) | Document workflows, handoffs, bottlenecks, and improvement opportunities. |
| [Project Coordinator](./skills/project-coordinator/SKILL.md) | Track scope, owners, milestones, risks, and status updates. |
| [Meeting Assistant](./skills/meeting-assistant/SKILL.md) | Prepare agendas and convert notes into decisions, actions, and owners. |
| [Customer Support Assistant](./skills/customer-support-assistant/SKILL.md) | Draft accurate, empathetic responses using approved product information. |
| [Incident Coordinator](./skills/incident-coordinator/SKILL.md) | Organize incident timelines, communications, and follow-up actions. |

## Product, design, and business

| Skill | What it helps with |
|---|---|
| [Product Manager Assistant](./skills/product-manager-assistant/SKILL.md) | Shape problem statements, requirements, user stories, and acceptance criteria. |
| [UX Research Assistant](./skills/ux-research-assistant/SKILL.md) | Plan research, synthesize supplied findings, and identify unanswered questions. |
| [UX and Interface Designer](./skills/ux-and-interface-designer/SKILL.md) | Create user flows, wireframe descriptions, and interface specifications. |
| [Brand and Content Assistant](./skills/brand-and-content-assistant/SKILL.md) | Maintain voice, messaging, and consistency across user-facing content. |
| [Marketing Planner](./skills/marketing-planner/SKILL.md) | Develop campaign briefs, content calendars, and channel-specific drafts. |
| [SEO Content Assistant](./skills/seo-content-assistant/SKILL.md) | Improve discoverability while prioritizing useful, accurate content. |
| [Sales Assistant](./skills/sales-assistant/SKILL.md) | Prepare account research, discovery questions, and proposal drafts. |
| [Business Analyst](./skills/business-analyst/SKILL.md) | Document business needs, requirements, options, and operational impacts. |
| [Finance and Budget Assistant](./skills/finance-and-budget-assistant/SKILL.md) | Organize budgets, explain calculations, and summarize financial scenarios. |
| [Hiring and People Operations Assistant](./skills/hiring-and-people-operations-assistant/SKILL.md) | Draft job materials, interview plans, onboarding guides, and internal communications. |

## Personal and specialist support

| Skill | What it helps with |
|---|---|
| [Personal Productivity Coach](./skills/personal-productivity-coach/SKILL.md) | Organize tasks and routines around the user's priorities and constraints. |
| [Travel Planner](./skills/travel-planner/SKILL.md) | Compare itinerary options using user-provided preferences and current source checks. |
| [Home and Event Organizer](./skills/home-and-event-organizer/SKILL.md) | Build checklists, schedules, and supply plans for everyday projects. |
| [Legal Information Organizer](./skills/legal-information-organizer/SKILL.md) | Summarize user-provided legal material and prepare questions for a qualified professional; not legal advice. |
| [Health Information Organizer](./skills/health-information-organizer/SKILL.md) | Explain general health information and help prepare clinician questions; not diagnosis or treatment. |
| [Safety and Risk Planner](./skills/safety-and-risk-planner/SKILL.md) | Identify practical risks, prevention steps, and escalation paths for ordinary activities. |

## Recommended foundation

Start with these cross-cutting skills in any setup:

1. **Task Planner** — clarify the outcome, constraints, and completion checks.
2. **General Researcher** — gather evidence and distinguish facts from assumptions.
3. **Workflow Automator** — use available tools deliberately and confirm consequential actions.
4. **Quality Checker** — verify the result against the request before reporting completion.
5. **Clear Communication** — explain results, limitations, and next steps plainly.

Then add only the specialist skills relevant to the work. For a software-focused setup, for example, add Software Builder, Debugging Assistant, Code Reviewer, Test Engineer, and Documentation Writer.

## Install for Hermes, Antigravity, or Claude Code

The skills are organized as `skills/<skill-name>/SKILL.md`. Install the **skill folder** (not just the Markdown file) into the location used by your agent. The examples below use a Unix-like shell; on Windows, you can copy the same folders with File Explorer or PowerShell.

### 1. Download the library

Clone this repository once:

```sh
git clone https://github.com/Jkmariner/ultimate-skills.git ~/ultimate-skills
```

If you already cloned it, skip this command. Choose a platform below. Install all 72 skills or copy only the skill folders you need. Before copying, check for existing folders with the same names so you do not overwrite local customizations.

### Hermes

Hermes loads user skills from `~/.hermes/skills/`. Copy all skills there:

```sh
mkdir -p ~/.hermes/skills
cp -R ~/ultimate-skills/skills/* ~/.hermes/skills/
```

Or install one skill directly from its `SKILL.md` URL:

```sh
hermes skills install \
  https://raw.githubusercontent.com/Jkmariner/ultimate-skills/main/skills/study-group-facilitator/SKILL.md \
  --name study-group-facilitator
```

Check installation with `hermes skills list` or `/skills`. Invoke a skill with `/skill-name` (for example, `/study-group-facilitator ...`). Newly installed skills may require a new session. See the [Hermes skills guide](https://hermesagent.nousresearch.com/docs/guides/work-with-skills).

### Antigravity

For one workspace, Antigravity uses `.agents/skills/`. From the root of your project:

```sh
mkdir -p .agents/skills
cp -R ~/ultimate-skills/skills/* .agents/skills/
```

Antigravity can also load user-level skills from `~/.gemini/config/skills/`. Skills can be selected automatically when relevant or invoked with `/skill-name`. See [Antigravity agent skills](https://antigravity.google/docs/skills) for the current locations supported by your Antigravity surface.

### Claude Code

For one project, install into `.claude/skills/` from the project root:

```sh
mkdir -p .claude/skills
cp -R ~/ultimate-skills/skills/* .claude/skills/
```

For personal use across projects, copy the folders into `~/.claude/skills/` instead. Claude can load a skill when relevant or when you invoke it as `/skill-name`. See [Claude Code skills](https://code.claude.com/docs/en/skills).

### Install only selected skills

Replace `study-group-facilitator` with a folder name from the catalog:

```sh
DESTINATION="$HOME/.hermes/skills" # set this to your platform's skills directory
mkdir -p "$DESTINATION"
cp -R "$HOME/ultimate-skills/skills/study-group-facilitator" "$DESTINATION/"
```

Change `DESTINATION` to the correct directory for your platform and scope: `~/.hermes/skills/`, `~/.gemini/config/skills/`, `~/.claude/skills/`, `.agents/skills/`, or `.claude/skills/`. Keep the copied folder name aligned with the `name` in its `SKILL.md`.

## How to use a skill

Skills are instructions, not fixed command-line programs. Give the agent a clear task and relevant context. Many platforms can select a matching skill automatically; you can also explicitly invoke one by its slash command:

```text
/student-study-coach I have two weeks before my biology and history exams.
Here are the topics and the hours I can study each day. Make a realistic plan
with review sessions and breaks.
```

```text
/academic-writing-coach Help me improve the structure of this draft.
Keep my ideas and voice, explain your suggested changes, and do not write
the assignment for me.
```

```text
/study-group-facilitator Plan a 60-minute study group for five students
reviewing cellular respiration. Include participation from everyone and
finish with a short knowledge check.
```

```text
/adaptive-agent-team Help me plan a student science fair project.
Use research, project-planning, and safety-review perspectives. Delegate
separate work only if this platform supports subagents; otherwise switch
perspectives yourself. Bring the findings together and flag anything
that needs my decision.
```

For better results, include:

1. **Goal:** what you want the agent to produce or help you accomplish.
2. **Context:** audience, course, project, source material, or current situation.
3. **Constraints:** deadline, length, tools, format, or boundaries.
4. **Success criteria:** what a useful result should include.

You can ask the agent to combine skills for a larger task, for example: “Use Technical Researcher to gather and cite current sources, then use Report Writer to create a concise brief from those findings.” The agent still needs appropriate tools and permission for tasks that access files, the web, or external services.

## Update, troubleshoot, and validate

Update your local clone with:

```sh
git -C ~/ultimate-skills pull --ff-only
```

If a skill is not available, check that its directory contains `SKILL.md` directly, the skill folder is in the correct platform directory, and the folder name matches the frontmatter `name`. Refresh or restart the agent session if needed. Avoid overwriting customized skill folders when updating.

The release skills follow the [Agent Skills specification](https://agentskills.io/specification). To validate one locally with the reference validator:

```sh
pipx run --spec 'git+https://github.com/agentskills/agentskills.git#subdirectory=skills-ref' \
  skills-ref validate ~/ultimate-skills/skills/study-group-facilitator
```

All 72 skill folders passed the Agent Skills reference validator (`skills-ref`). Platform-specific behavior can vary, so consult the linked official guides if a skill is not discovered or invoked as expected.

## License

The skills in this repository are provided under the [MIT License](./LICENSE).
