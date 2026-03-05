# Claude Code for Marketers — Course Outline

Audience: Complete beginners (no prior experience with code editors or terminals).
Format: Markdown with `[Screenshot: description]` placeholders for visuals.

---

## Intro: What Is Claude Code & Why Should You Care?

**Goal:** Set the stage before any setup — explain what this is, why it matters for marketers, and reframe the mental model.

### Section 1 — What Is Claude Code?
- An AI assistant that lives inside your code editor
- You describe what you want in plain English — it does the work
- It's not just for coding: research, writing, data analysis, content ops, file management, automation
- It's not ChatGPT — it reads your files, creates new ones, runs commands, and builds real things on your computer

### Section 2 — The Mental Model
- "You're not learning to code. You're learning to direct an AI that does the work for you."
- Your job: know what you want, describe it clearly, review the output, give feedback
- Claude Code's job: write code, create/edit files, run commands, fix its own mistakes
- Analogy: like managing a very fast, very literal junior team member

### Section 3 — What Can a Marketer Do With This?
- **Build things:** landing pages, campaign microsites, ROI calculators, internal tools, interactive presentations
- **Research & analyze:** competitive analysis, SEO audits, data cleanup & formatting, pipeline modeling, survey analysis
- **Write & automate:** bulk content generation, email sequences, meeting note summaries, report generation, file organization
- Frame broadly — this is not a coding tool, it's a work tool

---

## Module 1: Getting Set Up

**Goal:** Go from zero to sending your first prompt in Claude Code.

### Section 1 — Get VS Code
- One-sentence explanation of what VS Code is and why we use it ("It's a free app that gives Claude Code a home to work in")
- Steps: go to the download page, download for your OS, install, open it
- Screenshot placeholders at key moments
- Checkpoint: "You should see a Welcome tab"

### Section 2 — Add Claude Code
- What the Claude Code extension is (one sentence)
- Steps: open the Extensions sidebar, search "Claude Code", click Install
- Sign-in / authentication step
- Checkpoint: "You should see the Claude Code icon in your sidebar"

### Section 3 — Your First Prompt
- Open the Claude Code panel
- Type a simple, marketing-relevant prompt (e.g., "Write me 3 subject lines for a spring sale email")
- Watch the response appear
- Checkpoint: "You just used Claude Code for the first time!"

---

## Module 2: Your New Workspace — VS Code, the Terminal & Files

**Goal:** Get comfortable navigating VS Code and understanding how projects are organized.

### Section 1 — What Is VS Code?
- One-sentence explanation ("a free app for working on projects — think Microsoft Word, but for code")
- VS Code ≠ Visual Studio (clear this up immediately)

### Section 2 — Finding Your Way Around
- The four areas that matter: Sidebar (file explorer), Editor (where files open), Terminal Panel (where Claude Code runs), Command Palette (search for anything)
- How to toggle panels open/closed
- Skip: secondary sidebar, minimap, advanced layout

### Section 3 — Files, Folders & Projects
- Files vs. folders (same as their computer's file system, applied to a project)
- "Opening a folder" = opening a project in VS Code (the #1 beginner mistake is opening a single file)
- Common file extensions: .html, .css, .js, .md, .json
- What a project folder typically looks like

### Section 4 — The Terminal (Don't Panic)
- What it is: "a text conversation with your computer"
- Why Claude Code uses it (CLI-first tool)
- They do NOT need to learn commands — Claude Code handles that
- Key concept: commands run, output appears, the prompt (`$` or `%`) means "ready"
- The one thing to memorize: Ctrl+C to cancel/stop

### Section 5 — Extensions & Setup
- What extensions are (apps for VS Code)
- How to install one (Extensions sidebar → search → Install)
- Recommended starter extensions: Prettier, Live Server, GitLens
- Settings to change right away: Auto Save (critical), Font Size, Theme, Word Wrap
- Why Auto Save matters for Claude Code specifically (it reads files from disk)

### Section 6 — Keyboard Shortcuts Worth Learning
- Top 7 shortcuts with Mac + Windows columns
- Grouped: Navigation (Command Palette, Quick Open, Toggle Terminal, Toggle Sidebar), Editing (Undo, Find, Find in All Files)
- "Start with Command Palette and Toggle Terminal. Add others as you go."

---

## Module 3: The Workflow — How to Talk to Claude Code and Get Results

**Goal:** Teach the core skill — the describe → review → refine loop, prompting, iteration, and how to see your work.

### Section 1 — The Core Loop
- Describe what you want → Claude Code does the work → you review the output → you give feedback → repeat
- This is the entire skill — getting good at describing and giving feedback
- Analogy: steering, not building

### Section 2 — Prompting Basics
- Vague vs. specific examples side-by-side
  - Bad: "Make me a landing page" → Good: "Create a landing page for our spring webinar. Headline: 'Master ABM in 30 Days.' Include a signup form and 3 speaker bios."
  - Bad: "Analyze this data" → Good: "Read the CSV in /data/leads.csv and tell me how many leads came from each source last quarter."
- Tips: be specific, give context, reference files, state the format, iterate don't start over
- "The first prompt doesn't need to be perfect — that's what the loop is for."

### Section 3 — The Iteration Loop
- Show a 3-round example of progressive refinement
  - Round 1: "Create a one-page summary of our Q1 marketing metrics from the spreadsheet in /data/"
  - Round 2: "Add a chart comparing MQLs by channel. Make the table sortable."
  - Round 3: "Change the color scheme to match our brand (navy and teal). Add our logo."
- Each round builds on the last — you're not starting over, you're steering

### Section 4 — Seeing Your Work
- How to actually view what Claude Code built, depending on what you asked for:
  - Webpage / HTML file → right-click → Open with Live Server (opens in browser)
  - Text file, CSV, or markdown → opens in VS Code, click the file in the sidebar
  - Summary or analysis → Claude Code shows the answer directly in the chat panel
  - Changes to an existing file → the file updates automatically, check the editor tab
- If you installed Live Server, previewing websites is one right-click away

---

## Module 4: Skills — Saved Workflows You Can Reuse

**Goal:** Understand what skills are, why they matter, and how marketers can use and create them.

### Section 1 — What Are Skills?
- A skill is a set of instructions saved as a file
- When you type `/skill-name`, Claude Code loads those instructions and follows them — like giving it a playbook
- Side-by-side: long prompt paragraph vs. `/competitive-analysis https://competitor.com` — same result, one line, repeatable

### Section 2 — Why Skills Matter
- Consistency — same quality output every time, not dependent on how well you prompt that day
- Speed — complex multi-step workflows triggered with one command
- Shareability — anyone on your team can use the skill without writing the prompt themselves
- Iteration — improve the skill once, everyone benefits
- Analogy: like email templates — write the perfect version once, then reuse and adapt

### Section 3 — Examples for Marketers
- **Research:** `/competitive-analysis`, `/seo-audit`, `/persona-builder`, `/content-strategy-audit`
- **Content:** `/blog-post`, `/email-sequence`, `/social-posts`, `/case-study`
- **Operations:** `/meeting-notes`, `/quarterly-report`, `/data-cleanup`, `/campaign-brief`
- Many already exist; others are simple text files you can write yourself

### Section 4 — How Skills Work
- A skill is a markdown file (`.md`) saved in a specific folder
- Where they live:
  - Project skills — in your project's `.claude/` folder (shared with the team)
  - Personal skills — in your home `~/.claude/` folder (just for you)
  - Installable skills — downloaded from others, added in one step
- Key insight: if you can write a good prompt, you can write a skill — it's the same thing, just saved to a file

---

## Module 5: Context OS — A Knowledge System That Compounds Over Time

**Goal:** Understand what a Context OS is, why it matters, and how to set one up so AI never starts from scratch again.

Source: [jacob-dietle/gtm-context-os-quickstart](https://github.com/jacob-dietle/gtm-context-os-quickstart)

### Section 1 — The Problem
- Every new AI session starts from scratch
- You re-explain your business, re-teach preferences, re-provide context
- Knowledge doesn't compound — it resets
- Analogy: like onboarding a new employee every single morning

### Section 2 — What Is a Context OS?
- A structured knowledge base that Claude Code reads automatically every session
- Instead of scattered docs and repeated explanations, knowledge is organized, linked, and persistent
- Without Context OS: copy-paste context, inconsistent outputs, knowledge in your head, new team members start from zero
- With Context OS: AI reads knowledge base automatically, consistent compounding outputs, knowledge captured and reusable, instant onboarding

### Section 3 — Two Layers of Knowledge
- **Layer 1: Atomic Knowledge** (`knowledge_base/`) — individual reusable concepts (your ICP, positioning, frameworks, product facts)
  - Each concept is its own file with metadata and tags
  - Linked to related concepts via wiki-links
  - Lifecycle: emergent → validated → canonical
- **Layer 2: Operational Docs** (`00_foundation/`) — strategic documents that compose Layer 1 (positioning docs, messaging guides, process playbooks)
  - Reference atomic concepts, don't redefine them
  - Synthesis docs summarize entire domains
  - Update once, everything downstream benefits
- Analogy: Layer 1 = individual Lego bricks. Layer 2 = the things you build with them.

### Section 4 — Key Files
- `CLAUDE.md` — navigation guide; AI reads this first every session
- `taxonomy.yaml` — your blessed tags (domains, node types, status values)
- `ontology.yaml` — how concepts relate to each other
- These are the "constitutional documents" of your Context OS

### Section 5 — What Marketers Use It For
- **GTM & Sales:** ICP profiles that persist, competitive intel library, objection handling patterns, win/loss analysis
- **Content & Messaging:** brand voice & tone guides, value prop frameworks, positioning documents, messaging by persona
- **Operations:** call transcript processing, meeting notes → knowledge, onboarding new team members, cross-team context sharing

### Section 6 — Getting Started (10 Minutes)
- Clone the quickstart repo: `git clone https://github.com/jacob-dietle/gtm-context-os-quickstart.git`
- Open in VS Code / Cursor with Claude Code
- Run `/quickstart` — guided setup that:
  1. Asks what your context OS is for (GTM, Product, Research)
  2. Creates directory structure
  3. Generates CLAUDE.md navigation guide
  4. Sets up taxonomy and ontology rules
  5. Processes your first piece of content
  6. Verifies it works
- Built-in commands after setup:
  - `/ingest` — process raw content (transcripts, docs, notes) into knowledge nodes
  - `/graph-health` — check system health and get recommendations

### Section 7 — The Compounding Effect
- Every piece of content you ingest makes the system smarter
- Once you solve a problem, you save it and reuse it forever
- Skills + Context OS together = repeatable workflows with persistent knowledge
- The more you use it, the less you have to explain — that's the whole point

---

## Module 6: GitHub 101 — Saving, Sharing & Not Losing Your Work

**Goal:** Understand version control concepts so they can collaborate and track changes confidently.

### Section 1 — Git vs. GitHub
- Git = software that tracks changes (runs locally, like "track changes" in Word)
- GitHub = website that hosts projects online (like "Google Drive for code")
- They are different things that work together

### Section 2 — Why Version Control Matters
- No more `final_v2_FINAL.docx`
- Every change tracked — who, what, when
- You can always go back
- Multiple people can work without overwriting each other

### Section 3 — The Core Concepts
- Repository (repo): a project tracked by Git
- Commit: a labeled save point with a description
- Branch: a parallel draft of your project (photocopy analogy)
- Merge: combining a branch back into the main version
- Push/Pull: uploading to / downloading from GitHub
- Clone: downloading a project from GitHub for the first time
- Pull Request (PR): a formal proposal to merge changes, with review

### Section 4 — When Would a Marketer Use This?
- Collaborating on website changes
- Tracking content revisions
- Reviewing and approving changes via PRs
- Working with developers on the company site
- Building a personal/team site via GitHub Pages
- Claude Code handles the Git commands — you need the concepts to give good instructions

---

## Module 7: Key Concepts — Permissions, CLAUDE.md & Web Basics

**Goal:** Understand how Claude Code works and get a conceptual grasp of web technologies before building anything.

### Section 1 — Claude Code's Permission System
- Claude Code asks before it acts (edits files, runs commands)
- Saying "no" is always safe
- Almost everything is reversible (especially with Git)
- They can allow certain actions to skip future prompts
- This is a safety feature, not an annoyance — like a colleague confirming before making changes

### Section 2 — The CLAUDE.md File
- What it is: a briefing document for Claude Code that lives in your project folder
- Why it matters: the single most impactful thing you can write
- What to put in it: project description, goals, preferences, things to avoid
- It's just a text file — they already know how to write one
- Analogy: onboarding a new team member every time a conversation starts

### Section 3 — HTML, CSS & JavaScript (What They Do, Not How to Write Them)
- HTML = structure and content (the skeleton)
- CSS = styling and design (the clothing)
- JavaScript = behavior and interactivity (the muscles)
- These three work together on every website
- Knowing this helps them give Claude Code better instructions ("change the font" = CSS, "add a new section" = HTML, "make this button do something" = JS)

### Section 4 — Local vs. Remote vs. Live
- Local: files on your computer (where you and Claude Code work)
- Remote: files on GitHub (where you back up and collaborate)
- Deployed/Live: a website on the internet (a separate step)
- These are three different things — changing one doesn't automatically change the others

### Section 5 — Packages & Dependencies
- Modern web projects use pre-built code (packages/libraries)
- When Claude Code runs `npm install`, it's downloading these
- `node_modules` folder = thousands of files, this is normal
- `package.json` = the recipe list; `node_modules` = the ingredients
- Never edit `node_modules` directly

---

## Module 8: Working Together — GitHub as Your Team's Shared Workspace

**Goal:** Understand how to use GitHub (via Claude Code) to save your progress, collaborate with teammates, and never lose or overwrite each other's work — even when nobody on the team writes code.

### Section 1 — Why You Need This (Even If You're Not a Developer)
- You're using Claude Code to build landing pages, analyze data, create reports, manage a Context OS, write content — real work product lives in files now
- Without a system: you overwrite each other's changes, lose work, or end up with "which version is the latest?" chaos
- GitHub solves this the same way Google Docs solved document collaboration — but for entire projects
- Claude Code handles the Git commands for you. Your job is understanding the concepts so you can give good instructions.
- Analogy: Git is the "track changes" system. GitHub is the shared drive. Claude Code is the person clicking the buttons for you.

### Section 2 — Saving Your Progress (Commits)
- A **commit** = a labeled save point — a snapshot of your project at a moment in time
- Every commit has a short description ("Updated Q1 metrics report," "Added competitor analysis for Acme")
- You can always go back to any previous commit — nothing is ever truly lost
- How it works in practice: you finish a chunk of work → tell Claude Code "commit this with the message 'finished Q1 pipeline report'" → done
- Commit often — think of it like pressing save, but with a description of what changed
- Analogy: like bookmarking a page in a notebook with a sticky note that says what's on that page

### Section 3 — Working in Parallel (Branches)
- A **branch** = your own copy of the project where you can make changes without affecting anyone else
- The **main branch** is the "official" version — the source of truth
- You create a branch, do your work, and merge it back when you're done
- Why this matters for marketing teams:
  - Sarah is updating the messaging framework while Mike is building a new landing page — neither blocks the other
  - You can experiment freely on a branch — if it doesn't work out, just delete the branch
- Tell Claude Code: "Create a new branch called 'q2-content-refresh'" → work on it → merge when ready
- Analogy: like photocopying a document to try edits — if you like them, you replace the original. If not, you toss the photocopy.

### Section 4 — Sharing & Syncing (Push, Pull, Clone)
- **Push** = upload your local changes to GitHub (so teammates can see them)
- **Pull** = download the latest changes from GitHub (so you're up to date)
- **Clone** = download the entire project from GitHub for the first time (new team member getting set up)
- The daily rhythm: pull before you start working → do your work → commit → push when done
- Tell Claude Code: "Push my changes" or "Pull the latest" — it handles the rest
- If you forget to pull and someone else changed the same file, Git will flag a **conflict** — Claude Code can help you resolve it

### Section 5 — Reviewing Each Other's Work (Pull Requests)
- A **Pull Request (PR)** = "Hey team, I made some changes on my branch — can someone review before we merge?"
- PRs are how marketing teams can review each other's work before it becomes official
- Use cases:
  - Reviewing a new competitor analysis before adding it to the knowledge base
  - Checking messaging updates before they go into the Context OS
  - Approving a landing page before it goes live
- You can comment, request changes, or approve — just like reviewing a Google Doc
- Claude Code can create PRs for you: "Create a pull request with the title 'Updated ICP profiles for Q2'"

### Section 6 — A Real Example: Marketing Team Workflow
- Walk through a concrete scenario with a 3-person marketing team sharing a Context OS:
  1. Everyone clones the repo on Day 1
  2. Monday: Sarah pulls latest, creates a branch "sarah/blog-calendar," adds the Q2 content calendar, commits, pushes, opens a PR
  3. Tuesday: Mike reviews Sarah's PR, leaves a comment, approves it, Sarah merges
  4. Wednesday: Alex pulls latest (now includes Sarah's content calendar), creates a branch "alex/competitor-update," updates three competitor profiles, commits, pushes, opens a PR
  5. The main branch always has the team's latest approved work
- Key insight: nobody typed a single Git command — Claude Code did it all from plain English instructions

### Section 7 — Common Situations & What to Tell Claude Code
- "I want to save my work" → "Commit my changes with the message '[description]'"
- "I want to start working on something new without messing up what we have" → "Create a new branch called '[name]'"
- "I'm done, share it with the team" → "Push my changes and create a pull request"
- "I want to get my teammate's latest work" → "Pull the latest changes from main"
- "I messed something up and want to go back" → "Revert to the last commit" or "Undo my last commit"
- "Someone else changed the same file I changed" → "Help me resolve this merge conflict"

### Section 8 — Things to Know
- **Don't put secrets in the repo** — API keys, passwords, `.env` files should be in `.gitignore`
- **Commit messages matter** — "updated stuff" is useless in 3 months. "Added Q1 pipeline model with channel breakdowns" is useful forever
- **Pull before you push** — avoids most conflicts
- **The main branch is sacred** — always work on a branch and merge via PR
- Checkpoint: you can now save, share, collaborate, and recover — all through Claude Code in plain English

---

## Module 9: When Things Go Wrong — Recovery & Confidence

**Goal:** Build confidence by normalizing mistakes, addressing fears, and teaching practical recovery.

### Section 1 — "I See Code and I'm Scared"
- You don't need to read the code — you review the output
- If Claude Code built a page, look at the page, not the code behind it
- If Claude Code wrote a summary, read the summary
- The code is Claude's problem. The result is yours.
- Analogy: you don't need to understand a car engine to know whether it drove you to the right place

### Section 2 — Practical Recovery Options
- Claude Code did something you didn't want → Cmd+Z / Ctrl+Z to undo in the file
- A file looks completely wrong → tell Claude Code: "Undo your last change to [filename]"
- Everything feels broken → start a new Claude Code conversation (fresh context, fresh start)
- Want to go back to a known good state → if using Git, Claude Code can revert to any previous commit
- Something is running and won't stop → Ctrl+C in the terminal to cancel
- Almost nothing is permanent — the whole system is designed for safe experimentation

### Section 3 — Common Beginner Moments (This Is All Normal)
- "Claude Code is asking me to approve something I don't understand" → it's okay to say no; ask Claude Code to explain what it wants to do first
- "There are thousands of files I didn't create" → that's `node_modules`, totally normal, ignore them
- "The terminal is showing a wall of text" → Claude Code is working, let it finish; if stuck, Ctrl+C
- "I don't know if it worked" → ask Claude Code: "Did that work? Show me the result."

---

## Parking Lot

_Topics to work into the course — placement TBD._

- How to think about skills vs agents (skills covered in Module 4, agents TBD)
- The "Remotion" skill
- Intro to MCPs and how they work with Claude Code
- The importance of clean data
- CLAUDE.md best practices: global vs project level
- Running parallel agents (multiple Claude Code instances working on separate tasks at once)
- Advanced Context OS patterns: multi-agent orchestration, team governance, enterprise taxonomy

### From Boris (Claude Code Creator) — [Source](https://x.com/i/status/2007179832300581177)

- **Run multiple Claude sessions at once.** Think of it like having several assistants working on different tasks at the same time. Boris runs 5 in his terminal and 5–10 on the web. Each one works on its own copy of the project so they don't step on each other. _(ELI5: Imagine 10 kids each coloring their own copy of the same coloring book — nobody fights over crayons.)_

- **Use Plan mode before building.** Before Claude writes anything, switch to Plan mode (Shift+Tab twice) and go back and forth until you like the plan. Then let Claude build it. _(ELI5: Before you start building with Legos, draw a picture of what you want first. Then building is way easier.)_

- **Keep a shared CLAUDE.md and update it constantly.** Every time Claude does something wrong, add a note to CLAUDE.md so it doesn't repeat the mistake. The whole team contributes. _(ELI5: It's like a "house rules" list on the fridge — every time someone breaks a rule, you write a new one so everyone knows.)_

- **Use slash commands for things you do repeatedly.** If you find yourself typing the same kind of instruction over and over, save it as a slash command. Boris uses one for commit-push-PR dozens of times a day. _(ELI5: Instead of explaining your sandwich order every time, you just say "the usual" and the person already knows.)_

- **Use subagents to automate common workflows.** Boris has subagents for things like simplifying code after Claude is done, and for testing the app end to end. _(ELI5: After one kid finishes building, another kid checks the work and cleans up the mess.)_

- **Pre-allow safe permissions instead of skipping them entirely.** Use `/permissions` to approve commands you know are safe, rather than turning off the safety system altogether. _(ELI5: Instead of leaving the front door wide open, you give house keys to people you trust.)_

- **Give Claude tools to verify its own work — this is the #1 tip.** If Claude can see the output of what it built (run the server, view the page, run tests), the quality jumps 2–3x. _(ELI5: If you bake a cake but never taste it, you won't know if it's good. Let Claude taste the cake.)_

- **Use hooks to auto-format code.** A PostToolUse hook can automatically clean up formatting after every change, catching the last 10% that Claude misses. _(ELI5: Like spell-check that runs automatically every time you finish typing a sentence.)_

- **Use Opus with thinking for best results.** Even though it's slower, you spend less time steering and correcting, so it's faster overall. _(ELI5: The slow, careful kid finishes the puzzle faster because they don't have to redo pieces.)_

- **One task per session, separate git checkouts.** Each Claude instance works on one thing in its own copy of the project. To roll back a mistake, just press Esc twice. _(ELI5: Each kid gets their own desk and their own copy of the homework — if one kid messes up, the others aren't affected.)_

- **Use Claude Code's GitHub Action for code review.** Tag `@.claude` on PRs to have Claude review code and suggest CLAUDE.md updates as part of the review process. _(ELI5: Before your homework gets graded, your robot study buddy checks it first and fixes the obvious mistakes.)_

- **Don't sit and watch — steer and check in.** Especially on the web, kick off tasks and come back to them. Boris starts sessions from his phone in the morning and checks later. _(ELI5: You put clothes in the washing machine and go do other stuff — you don't stand there watching it spin.)_

- **Let Claude use your other tools via MCP.** Claude can search Slack, run database queries, grab error logs, etc. — all through MCP integrations shared with the team. _(ELI5: Instead of running to the library yourself, you tell your assistant where the library is and they go look stuff up for you.)_

### To-Do: Gather Input
- [ ] Michal at Orchestry — tips and best practices
- [ ] Joe Rhew — tips and best practices
- [ ] Jacob Dietle — tips and best practices
- [ ] Jordan Crawford — tips and best practices
