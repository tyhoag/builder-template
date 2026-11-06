# Sprint 1 Review

**Window:** 2026-10-26 to 2026-11-06
**Sessions reviewed:** 1 across 1 project (Claude Code 1, Codex 0; 0 sessions excluded at your request)
**Not visible to this review:** The team's master repo (project MENA) and the Claude Code and Codex sessions that worked in it. The Claude artifact prototype. Work on the PRD. Getting access to the WhatsApp API. The scan only saw this repo, and its one session was the one that wrote this review.

## Where the work lives

| Item | What it is | Commits in window | Shared with sdmurff |
|---|---|---|---|
| `tyhoag/builder-template` (this repo) | Sprint plan, README and CLAUDE.md context | 1 (2026-10-26: "Sprint 1 plan; fill in README and CLAUDE.md context") | Not confirmed |
| Team master repo (MENA) | All team code, per the builder | Not visible to this review | Not confirmed |
| Claude artifact prototype | Prototype of the product, per the builder | Not applicable (no repo) | No link recorded |
| WhatsApp test number | Not live. The builder has access to the WhatsApp API | Not applicable | Not applicable |

## When you worked

In this repo: 2 days with commits or sessions out of 14 (Oct 26 for the plan, Nov 6 for this review). Work in the master repo and in other tools is not visible, so the shape of the whole sprint cannot be stated.

## Where you got stuck

Nothing visible in this repo's sessions. The one session in the window is this review. Stuck points in the master repo or in Codex sessions are not visible to this review.

## What took the most time

Not determinable from this repo. The one visible session was 3 prompts, all about this review. The builder reports that most of the sprint's work was done in Claude Code, with some in Codex, in the master repo.

## Builder tools you used

| Building block | What it is | This sprint (this repo only) |
|---|---|---|
| Skills you wrote | Skills you made yourself | not used |
| Course skills | sprint-plan, sprint-review, sprint-coach, learn, eli5 | sprint-review (1) |
| Plugins | Skills or subagents from a plugin | not used |
| Slash commands | Commands typed with / | sprint-review (1) |
| Hooks | Scripts the harness runs on events | not used |
| Subagents, named | Defined in `.claude/agents`, by a plugin, or by you | not used |
| Subagents, built-in | Ship with Claude Code; Claude may start them | not used |
| Messages to other sessions | Messages to subagents or other sessions | not used |
| Plan mode | Plan tool calls and turns in plan mode | not used |
| Permission mode | Raw mode names, turns in each | auto (1) |
| Permission prompts and denials | Prompts answered, calls a rule or check denied | allowed by a permission rule (1) |
| Where sessions ran | Interactive, `claude -p`, desktop app, VS Code | remote_desktop (1) |
| Worktrees | Separate git worktrees | not used |
| Memory and instructions | Files loaded and edited | CLAUDE.md loaded (1); none edited |
| Reaching outside the repo | Service CLI tools, MCP servers and connectors, direct API calls | none used in the scanned session |

Not used this sprint (in this repo's scanned session): hooks, subagents, plan mode, worktrees, MCP servers, service CLI tools, direct API calls. Codex sessions do not show these, and the builder's Codex sessions were not scanned.

Scan version: sprint_scan 2026-10-16.

## Users this sprint

No outside users this sprint.

## Learning sessions

None logged this sprint. You studied no axes through `/learn`; the sprint's work was Design (see Axis).

## Axis

**Design.** By the builder's account the sprint's work was the PRD and a Claude artifact prototype, which is spec and interface work; this is the builder's description, not something the scan could confirm.

## Against your plan

**Goal was:** Get early signal from interviews with mentors in Colombia, plus a working WhatsApp prototype for them to react to, so we can judge whether Mentors International's entrepreneurs would use a WhatsApp teaching curriculum.

**Done looks like (plan):** A test WhatsApp number (built on Meta's API) that anyone can message, in text or by voice memo, to get lesson 1, and that replies in text, plus joining some of the mentor interviews in Colombia.

- **WhatsApp test number:** Not live. The builder has access to the WhatsApp API. The prototype that exists is a Claude artifact, not a WhatsApp number, so nobody can message it on WhatsApp.
- **Interviews:** No interview calls have happened yet and the builder was not part of any. `discovery/interviews/` contains only the template.
- **Early signal:** None collected.

---

## Your retro

*The builder's own answers, recorded word for word. Dictation errors were corrected at the builder's request: "Claude artifact prototypes", "API", and "slightly less difficult" in the difficulty answer.*

**Did you hit the goal?**
I would say the goal changed a little bit because we're part of the more robust team with multiple different roles and a lot more executive oversight. Those goals have kind of shifted in the last two weeks. We've only been making Claude artifact prototypes, which is fine. We've started pretty extensively on some actual prototype that we'll work within WhatsApp.

Our prototype has been more of a question of if it's even the right thing to build, or if it's answering the right pain point. We've had lots of meetings with our mentors and the international team to decide if it's even been the right decision. I would say we've partially completed that goal in terms of we know now better what they want us to build and how it will actually work for them.

We do have WhatsApp API access for one member of my team. We're working on getting it for the rest of the development team so that we could get rid of that blocker.

**What did the report show you?**
Yeah, I'm not committing anything to this repo. I don't know if that was really surprising to me. I'm not seeing anything here. I thought that was just doing my sprint logging here more than anything.

No, I haven't been. That's a fine report. I'm not actually adding anything to this repo.

**If the plan changed, why?**
Yes and no. It's changed because we're constantly pivoting to figure out if what we're building is actually what the team wants. And so that executive oversight has been challenging, but good, because it holds us accountable to a standard of quality that we need and our clients need, those who depend on Mentors International to deliver a good product. I think building the correct thing is a lot more important than building something quickly.

**Actual difficulty:**
Yeah, I would say of 3.5.

I think it was slightly less difficult. And for a different reason, it was difficult because it was of the executive input and oversight that have made it more difficult, rather than just the complexity of the challenge that we're trying to overcome.

**What will you change next sprint?**
Better, more defined roles from the team. We've already talked about this in our meetings. Isn't something if you're real. We've actually talked about that.

In the next sprint, we want to get an actual working product that you can text on WhatsApp, not just a clunky artifact. The prototype. And, yes, the whole dev team should get WhatsApp API access.
