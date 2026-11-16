# Mentors International: WhatsApp Teaching Prototype

> A WhatsApp chatbot that delivers a teaching curriculum to Mentors International's entrepreneurs in Colombia (pilot in Colombia or Mexico).

**Where to see it:** The team repo and project board under Work files and links below, and the sprint demo on Loom (the WhatsApp number is a Meta test number until MI's business account is verified)
**Built by:** tyhoag, AI Foundry, BYU

## Context

- **My role:** One of two AI engineers on the Mentors International project team. My hats are
  AI builder, researcher, and team member. I help decide what to build and the most feasible way
  to build it, and I build the prototypes that test those choices.
- **What I am working on:** My part of the team's product: prototypes for a WhatsApp teaching
  curriculum, starting with a bot that delivers lesson 1 by text. The team (a designer, two
  product managers, a head of development, and an executive team we answer to) already has a PRD
  and several Claude artifact mock-ups; this work moves to something usable inside WhatsApp.
- **Who it is for:** Entrepreneurs in Colombia whom Mentors International serves.
- **Who uses my work:** My teammates and the Mentors International executive team, who will
  react to the prototype and decide whether to run a pilot. Mentors in Colombia are also
  interviewed to see whether they would use it.

Mentors International content is under NDA. Lesson content and internal documents stay out of
this repo.

## Work files and links

| What | Link | Access |
|---|---|---|
| Team code repo (Maia WhatsApp bot) | https://github.com/Ensign-College/mena-mockup-1 | Private. sdmurff invited as a read-only collaborator on 2026-11-16 |
| Team project board (Maia Q&A V1) | https://github.com/orgs/Ensign-College/projects/43 | Ensign-College org project |
| Development backlog I set up (Sprint 2 operations work) | [Issues #4 to #52](https://github.com/Ensign-College/mena-mockup-1/issues?q=is%3Aissue+author%3Atyhoag) | In the team repo. I wrote all 49 on 2026-11-10: decisions (#4 to #8, #50, #51), build work by area, blocked ops items, and a parking lot |
| My PR: save how long the socio waited for each answer | [PR #61](https://github.com/Ensign-College/mena-mockup-1/pull/61) (closes #23) | In the team repo; 5 commits by tyhoag, with tests |
| WhatsApp buttons (Sprint 2 build work, in progress) | [#11](https://github.com/Ensign-College/mena-mockup-1/issues/11) privacy "I agree" buttons, [#12](https://github.com/Ensign-College/mena-mockup-1/issues/12) topic buttons, [#16](https://github.com/Ensign-College/mena-mockup-1/issues/16) thumbs rating | Issues in the team repo; the PR link for each goes here when it opens |
| Team PRs I reviewed | [PR #1](https://github.com/Ensign-College/mena-mockup-1/pull/1) (merged 2026-10-31), [PR #2](https://github.com/Ensign-College/mena-mockup-1/pull/2) (approved 2026-11-05) | In the team repo |
| Claude artifact prototype (Sprint 1 demo) | https://claude.ai/artifact/Bg4SnEmzGQk5R7X32Wz2tx | Public: anyone with the link can open it |
| Sprint plans and reviews | `sprints/` in this repo | Public in this repo |
| Team PRD | Not linked | Under Mentors International's NDA, so it cannot be shared |
| WhatsApp test number | Not public | Runs on the team's Meta test number; Meta business verification (team issue #37) is still pending, so it only reaches registered test phones. The Sprint 2 Loom shows it on a test phone |

Mentors International content and documents are under NDA and stay out of this repo. My code
work happens in the team repo above, not here; this repo holds sprint plans, reviews, and notes.

## What is in this repo

| Folder | What lives here |
|---|---|
| `sprints/` | One plan and one review per sprint |
| `discovery/` | Interviews, personas, what you learned about your user |
| `design/` | Flows, screens, usability test notes |
| `product/` | The work itself: code, a pricing model, a copy deck, an automation |
| `specs/` | One spec per piece of work, written before you make it |
| `gtm/` | Launch, channels, copy, experiments |
| `metrics/` | What you measure and what it says |
| `decisions/` | Numbered records of what you decided and why |
| `learning/` | One log per `/learn` session: what you explained, what you missed, what you still wonder |

Not everyone in this course writes software. An interview, a pricing model, a landing page
draft, and a usability finding are all artifacts, and they get committed like anything else.
Use the folders that fit your role and ignore the rest.

If you build an AI feature, put its eval set in `product/evals/`. A test set is how you know
whether a change to a prompt helped or hurt.

## Running it

[If your work includes code: how to run it locally. Delete this section if it does not.]

## Sprints

Each sprint:

```bash
/sprint-plan     # start of the sprint: commit the plan, submit it on Canvas by Wednesday
# ...do the work...
/sprint-review   # on or before the Monday the sprint ends: writes the report, asks your five retro questions, then commit
# when your sprint report arrives: press Copy prompt in it and paste the prompt into Claude Code;
# the sprint-coach skill goes over the report with you and updates your next plan
```

## Learning a section

Sections of the [course book](https://byu-strategy.github.io/product-management/) that teach a
model have a **Learn in Claude** button beside their heading. It copies a prompt; paste it into
Claude Code for a tutoring session on that section. Bring your own questions, or let Claude lead,
and say "quick" or "go deeper" whenever you like. It ends with a short check and commits a log to
`learning/`. To learn one builder concept, give its id: `/learn DE02` teaches the passage for
concept DE02. Your sprint report links each concept it lists to its passage.

When an idea will not click in words, type `/eli5 <the idea>` (or say "explain it like I'm
five"). Claude draws a one-page picture of it with very few words and gives you a link to open
it (or, if it cannot make a link, saves it under `learning/eli5/` and tells you where). `/learn`
offers this on its own when you get stuck.

## Update your course skills

The course skills (`/sprint-plan`, `/sprint-review`, `/sprint-coach`, `/learn`, `/eli5`) live in
`.claude/skills/`. They change during the semester. When the course or your sprint report asks you
to update them, open Claude Code in this repo and paste this:

```text
Update my course skills from the class template. Clone https://github.com/byu-strategy/builder-template (main branch) into a temporary folder outside this repo with `git clone --depth 1`. For each folder in the template's `.claude/skills`, replace the folder with the same name in this repo's `.claude/skills` with the template's copy, and add any that are missing. Do not change any other skill or any other file in this repo. Delete the temporary folder, then commit only `.claude/skills` with the message "Update course skills" and push. Then tell me to start a new Claude Code session so the updated skills load.
```

It copies every course skill from this template into your repo and leaves the rest of your repo
as it is. A skill you wrote yourself keeps working, unless you gave it the same name as a course
skill.

## Ground rules

- **Spec before work.** For anything non-trivial, the spec's commit should predate the
  work's commits.
- **Decisions get recorded.** When you make a real choice, write it in `decisions/` with the
  alternatives you rejected.
- **No real customer contact details anywhere in this repo.** Anonymize people in interview
  notes: "dental office manager, Provo" rather than a name and an email.
- **Keep `CLAUDE.md` current.** It is what your agent knows about your work. Stale context
  produces bad output.
