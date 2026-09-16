# Beyond the Ivory Tower

[简体中文](README.md) | English

> Turn what you have done into a resume, a portfolio, and clear stories for your job search.

[![Version](https://img.shields.io/badge/version-v1.0.0-2563EB.svg?style=flat-square)](VERSION.md)
[![License](https://img.shields.io/badge/license-MIT-16A34A.svg?style=flat-square)](LICENSE)

**An AI job search toolkit for students entering work and recent graduates reconsidering their direction.**

Find evidence of your skills in coursework, student activities, internships, and work. Compare roles, create resumes and portfolios, and prepare for interviews. As your experience grows, use the same methods for job changes and career transitions.

**For Claude Code, Codex, and other tools that support Agent Skills. Free and open source.**

[Quick start](#quick-start) · [What it helps with](#what-it-helps-with) · [Guide](docs/guide.en.md) · [Skill directory](docs/skill-inventory.en.md) · [Installation and updates](docs/install.en.md)

![From experience to job search materials](docs/career-assets-flow.en.svg)

**Start with `zane-career-assets` and describe the task at hand.** It selects the methods needed for your task. You can begin with the material you already have.

<a id="install"></a>

## Quick start

### 1. Install

Run in your terminal:

```bash
npx -y skills add ZanePan2027/zane-career-skills -g --all
```

Or ask your Agent:

```text
Install all Skills from https://github.com/ZanePan2027/zane-career-skills.
Then use zane-career-assets to help me with this: ...
```

Select your Agent in the installer, then reload Skills if required. The terminal command requires Node.js and `npx`. Omit `-g` to install for the current project; see the [installation guide](docs/install.en.md) for updates.

### 2. Describe the task

```text
Use zane-career-assets.
I am preparing for my first job. I completed a course project and managed
registration and check-in for a student event. Here are my report and notes.
Help me identify what belongs on my resume, then compare what to emphasize
for these two roles.
```

A useful first result is a set of relevant experiences, your contribution, facts to clarify, and role-specific resume bullets. Share an existing resume or job description if available. You can also begin by describing one thing you have done.

### 3. Continue with a draft or practice

```text
Turn this experience into a resume bullet.
Then practice an interview about it. Ask one question at a time and wait for my answer.
```

For a complete resume, portfolio, or website, specify the role, language, and files you need. The same entry also handles a single focused task.

## What it helps with

| What you can say | What you can get |
| --- | --- |
| I have no internship. Can a course project go on my resume? | Your actions, work samples, and supported resume bullets |
| What evidence do I have for each of these two roles? | A comparison of requirements, strengths, and missing evidence |
| I have an old resume and want to apply in English | Content and layout adapted to the role and hiring market |
| My project answer sounds like a list of events | A clear answer, with follow-up questions and revisions |
| We worked as a team. How do I describe my contribution? | A distinction between your actions and team results |
| I want a portfolio to show my projects | Reading structure, case content, and a website implementation |

## From experience to application materials

The Agent organizes facts and evidence from your experience, then uses the target role to decide what to emphasize. Resumes, portfolios, application messages, and interview answers draw on that evidence.

When continuing the same project, bring back corrections or hiring feedback. The Agent checks which materials are affected, updates them, and explains what changed. Producing and checking Word, PDF, or website files uses the tools available in your Agent environment.

[Follow a complete example: from a student event to a resume and interview](docs/guide.en.md)

## Continue a previous task

Keep the work in a project folder you choose. Before pausing, ask the Agent to save the selected version, outstanding facts, and next step. Give a later session that folder and identify the application or interview practice to continue.

If the chat cannot read or write files, save a continuation note and provide it next time with the relevant material.

## Use a specific method

Start with `zane-career-assets`. Once familiar, you can directly select resume, portfolio, case writing, application messages, or delivery checks. The [Skill directory](docs/skill-inventory.en.md) lists situations, example requests, and outputs for all eleven entries.

## Choosing between the two toolkits

Start here to match experience to roles, create application materials, and practice interviews. For a choice involving family arrangements, finances, location, and personal direction, use [Live Your Life Well](https://github.com/ZanePan2027/zane-life-workbench) to weigh them together. Each toolkit works independently.

## Provenance and license

These methods grew from practical work on resumes, bilingual portfolios, project stories, and job applications, with continued attention to role relevance, consistency, and real feedback.

See [Provenance](docs/provenance.md) for design references. This repository uses the [MIT License](LICENSE).

Author: Zane
