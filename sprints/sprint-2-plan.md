# Sprint 2 Plan

**Menu:** Build for Mentors International, engineering (WhatsApp bot front end and interactive features) and operations (development task tracking)

**Teammates:** Another developer (bot logic), a development lead, two product managers, one student product manager, one main product manager, and a Colombia relationship lead.

**Goal:** The WhatsApp bot's interactive features and front end work. Users get buttons, built on one shared message framework, and starter-topic buttons start a lesson answer. The development team's task management is set up in GitHub issues.

**My part:** Front-end design and functionality of the WhatsApp bot: the buttons and the interactive side. The other developer owns the bot's logic. I also set up the GitHub issues the development team uses for task management.

**Who will see it:** The whole team will use it. The product managers will test the buttons in WhatsApp and read the GitHub issues to see the backlog and what the developers are working on. By the end of the sprint the Mentors International executive team (the CTO and one of their internal product managers) will also see it.

**Why this:** The bot currently replies to texts and voice notes but has no buttons or other interactivity. The team has prototyped with Claude artifacts and wants to find the best way to engage the mentees (socios) so they actually use it. A text-only bot would look like ChatGPT or any other tool they may already use; an interactive, user-friendly, somewhat gamified bot is more helpful to them.

**What done looks like:** The message framework for buttons, lists, links, images and carousels is merged (#150). The buttons are sent through the framework to a real phone and shown in the demo. The starter-topic buttons (#12) are built, tested and submitted for review in PR #154: a socio taps Empecemos, gets three topic buttons, taps one, and Maia answers that topic's question. They go live once a code owner approves the PR. The GitHub issues exist in the team repo so the product managers can see the backlog and what is in progress. Lesson delivery through quiz buttons (#13, #14) is not part of this sprint, and carousels exist only as framework helpers, not in a live flow.

**Predicted difficulty:** 3

**Changes:**
- Nov 19: replaced lesson delivery through quiz buttons with starter-topic buttons that start a lesson answer, because quiz buttons wait on #13 (the AI writing a quiz question with answer choices), which is not built yet.
- Nov 20: changed #12 from live in the bot to built, tested and submitted for review, because merging needs a code owner's approval and Michael can't approve before the deadline.
