# Sprint 2 Review

**Window:** 2026-11-10 to 2026-11-20
**Sessions reviewed:** 6 across 5 projects (Claude Code 6, Codex 0; 56 sessions excluded at your request)
**Active session time:** about 6.2 hours (gaps under 15 minutes). This counts only time with back-to-back activity in the 6 Claude Code sessions above. It leaves out the meetings, GitHub web reviews, the Meta dashboard, Slack, and any work outside Claude Code.
**Not visible to this review:** Team meetings, per the builder's calendar: a Mentors International check-in (Nov 10), the AI Mentor product manager meeting (Nov 10), the AI Mentor project team meeting (Nov 11), and the prep and MI executive review meetings (Nov 13). GitHub web reviews of teammates' PRs. The Meta dashboard. Slack threads with the team.

## Work files and links

| Repo | Commits by the builder in the window | Shared with sdmurff |
|---|---|---|
| `tyhoag/builder-template` (this repo) | 9: Sprint 2 plan (Nov 10), README work links (Nov 16, Nov 20), two plan changes (Nov 20) | Public |
| `Ensign-College/mena-mockup-1` (team repo) | 11 on the builder's own PRs, listed below | Invited as a read-only collaborator on 2026-11-16; invite not yet accepted |

Builder's commits in the team repo, by PR (dates, messages and PR numbers only):

| Date | PR | Commit message |
|---|---|---|
| Nov 16 | #61 | Save how long the socio waited for each answer (#23) |
| Nov 16 | #61 | Store: record and query the socio's reply wait (#23) |
| Nov 16 | #61 | Handler: save the socio's wait after each answer is sent (#23) |
| Nov 16 | #61 | Migration 0007: messages.reply_wait_ms (#23) |
| Nov 16 | #61 | Tests for the socio reply wait and its median (#23) |
| Nov 17 | #61 | Fix reply-wait tests failing on non-UTC machines (#23) |
| Nov 17 | #150 | Add the WhatsApp message framework and a payload preview (#53) |
| Nov 17 | #150 | Merge origin/main into the framework branch |
| Nov 17 | #153 | Run pytest on every PR and push to main (#152) |
| Nov 17 | #154 | Starter topic buttons after "Empecemos", behind a flag (#12) |
| Nov 20 | #154 | Merge main into 12-starter-topics (#12) |

PR status at the end of the window:

- **#150**, WhatsApp message framework (buttons, lists, links, images, carousels, `/preview`): merged Nov 17, approved by a teammate, 39 new tests.
- **#154**, starter-topic buttons (closes #12): open, 12 new tests, no conflicts with main. Waiting on the required code-owner approval. The `main` ruleset requires one approval and allows no bypass.
- **#153**, pytest GitHub Action (closes #152): open, its own pytest check passes, waiting on review.
- **#61**, reply wait time (closes #23): its commits reached main through integration PR #155.

Other activity in the team repo during the window:

- Issues #4 to #52 (49 issues) opened by the builder on Nov 10, and the "Maia Q&A V1" project board (github.com/orgs/Ensign-College/projects/43).
- Teammates' PRs merged by the builder: #54, #56, #145, #146, #147, #148, #149, #151, #155, #156.
- On Nov 17 and Nov 20 the framework's demo messages were sent from the team's Meta test number to the builder's phone and arrived. The Loom shows them.

## When you worked

5 days with sessions out of the 11 days in the window: Nov 10, 11, 16, 17 and 20. Most prompts came on Nov 10 (issues and the project board) and Nov 17 (the framework, CI and topic buttons). Nov 20 was spent on the wrap-up. There were no sessions Nov 12 to 15, the days of the Nov 13 executive review.

## Where you got stuck

1. **The backlog on Nov 10.** The first version of the issues read as unclear and machine-written. The builder asked whether they described work the codebase already did or work that was invented, asked for them to be checked against the PRD and the code, and reported that the project board showed none of the claimed changes. It ended with the issues rewritten in plain language, a board view, and a Fibonacci effort field the builder asked for.
2. **Vercel checks on Nov 17.** PRs showed a failing Vercel check the builder did not recognize. It ended when the builder merged #146 (the Vercel entrypoint) and the check passed.
3. **Getting #154 live on Nov 19 and 20.** #154 conflicted with main after the integration PR. The conflict was resolved, but the merge needs a code owner's approval and none was available before the deadline. The builder chose to change the plan rather than wait. Separately, the first live send to the phone on Nov 20 did not arrive. It arrived after the builder messaged the test number, which opened WhatsApp's 24-hour messaging window.

## What took the most time

By prompt volume and session size, Nov 17 in the `whatsapp-integration-prototypes` worktree: the message framework (#150), the CI workflow (#153), the starter-topic buttons (#154), and checking button rendering on the iOS Simulator and a real phone. Second was Nov 10 in the `mentors-intl-scope-definition` worktree: answering the PRD's open questions, writing the 49 issues, and setting up the project board.

## Builder tools you used

| Building block | What it is | This sprint |
|---|---|---|
| Skills you wrote | Skills you made yourself | not used |
| Course skills | sprint-plan, sprint-review, sprint-coach, learn, eli5 | none in the scanned sessions (this review is run with sprint-review) |
| Plugins | Skills or subagents from a plugin | not used |
| Slash commands | Commands typed with / | not used |
| Hooks | Scripts the harness runs on events | not used |
| Subagents, named | Defined in `.claude/agents`, by a plugin, or by you | web-fetch (1) |
| Subagents, built-in | Ship with Claude Code; Claude may start them | not used |
| Messages to other sessions | Messages to subagents or other sessions | not used |
| Plan mode | Plan tool calls and turns in plan mode | not used |
| Permission mode | Raw mode names, turns in each | auto (100) |
| Permission prompts and denials | Prompts answered, calls a rule or check denied | allowed by a permission rule (138), approved at a prompt (9), blocked by auto mode (1) |
| Where sessions ran | Interactive, `claude -p`, desktop app, VS Code | Claude desktop app (6) |
| Worktrees | Separate git worktrees | none recorded by the scan (the team-repo sessions ran in `.claude/worktrees` folders) |
| Memory and instructions | Files loaded and edited | CLAUDE.md loaded (user 9, project 7), AGENTS.md (2), MEMORY.md (2); none edited |
| Reaching outside the repo | Service CLI tools, MCP servers and connectors, direct API calls | CLI: gh (172), twilio (2), vercel (1). MCP: desktop task list (130), iOS Simulator (22), built-in browser (19), Claude Docs (9), PR status (7), Slack (4), session management (4), Granola (3), Vercel (2). Direct API calls: curl (4), http (1) |

Not used this sprint: your own skills, plugins, slash commands, hooks, built-in subagents, messages to other sessions, plan mode.

Scan version: sprint_scan 2026-10-16.

## Users this sprint

No outside users this sprint.

## Learning sessions

None logged this sprint. The sprint's work was Application Architecture (see Axis).

## Axis

**Application Architecture.** Most of the time went to integrating with the WhatsApp Cloud API: one validated layer that builds every interactive payload against Meta's limits, a tap router, a pytest CI workflow, and tests.

## Plan compared with the work

**Goal was:** The WhatsApp bot's interactive features and front end work. Users get buttons, built on one shared message framework, and starter-topic buttons start a lesson answer. The development team's task management is set up in GitHub issues.

The plan changed twice: on Nov 19 (quiz-button lessons replaced by starter-topic buttons, because quiz buttons wait on #13) and on Nov 20 (#12 changed from live in the bot to built, tested and submitted for review, because the merge needs a code owner's approval).

**Build for Mentors International, engineering (WhatsApp bot front end and interactive features):** The framework is merged (#150). Its buttons, list, image, link and carousel messages were sent to a real phone and arrived. The starter-topic buttons are built and tested in #154 and are not merged, so a tap on a topic button does nothing in the live bot yet. This matches the plan as changed on Nov 20. It does not match the plan as first written, which had lesson delivery through buttons working in the bot.

**Operations (development task tracking):** Matches. 49 issues and a project board exist in the team repo, and the team's PRs reference them (for example #12 to #154, #53 to #150, #23 to #61).

---

## Your sprint retrospective

*The builder's own answers, recorded word for word. Dictation errors were corrected at the builder's request: "GitHub issues" in the goal answer, and "WhatsApp frontend design for lesson delivery" in the plan-change answer.*

**Did you hit the goal?** Yes, I hit my goal in part. I was able to set up an extensive backlog and GitHub issues where we can track all the progress that we're making. It's been a fairly bureaucratic process, considering we have a large team, but I think we're finally making progress in terms of actually getting stuff done within the code.

**What did the client or your users say?** We will have a meeting about my work tomorrow at 12. That is when our team meetings are. They are after this sprint is due, so we will see.

**What did the report show you?** I think the most insightful part about the report is learning what I'm using and not using enough of during sprints. I don't feel like it's super accurate on a lot of these things, but it still is insightful to me to realize that I should be using more of all the builder tools as I work. I think it just helped me get perspective that there's a lot more stuff that I could be using to make my building a lot easier.

**If the plan changed, why?** Yes, I changed the plan. The only thing I really changed was because there was a blocker in getting my pull request approved, and I ran a prototype version of the WhatsApp buttons within an actual WhatsApp number. They actually sent, and the layout works correctly, but it wasn't connected entirely yet to the AI brain that makes it completely functional. Other than that, the plan stayed the same: to work on GitHub issues and WhatsApp frontend design for lesson delivery.

**Actual difficulty:** Honestly, I think it was a 4. It was actually a pretty hard sprint, mostly because working with the team can be frustrating at times, understanding expectations, and trying to juggle everything that I have going on. I would say the number of meetings that we had, mixed with the way that we've been operating, has made it difficult. Also, seeing my sprint reviews and reading through them sometimes makes me feel less competent, and so it makes me feel like it should have been easier than it was, which is sometimes frustrating.

**What will you change next sprint?** I just want to be more intentional about how I spend my time and what I accomplish because I feel like there's so much to get done. When you have a super large team for a project that doesn't feel as large as it is, you tend to get lost in the background at times. Just intentional with my work and more directed in my approach
