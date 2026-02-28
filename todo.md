# TODO.md — Execution OS

## 🔧 Friction Log (Manual Steps to Automate)

Track every manual step → "why manual?" → automate if >5min/week.

| Manual Step | Frequency | Time Cost | Automation Path | Status |
|-------------|-----------|-----------|-----------------|--------|
| gog Gmail auth setup | Weekly | 10 min | Export GOG_KEYRING_PASSWORD or cron reminder | ⚠️ |
| Copy-paste email draft | Daily | 2 min | message tool integration | ❌ |
| Browser tab attachment for X | Daily | 5 min | auto-attach workflow | ❌ |
| Manual session handoff notes | Daily | 3 min | auto-template from memory/YYYY-MM-DD.md | ⚠️ |
| Prediction logging for decisions | As needed | 2 min | progress-log.md template | ❌ |
| Friction logging | After every task | 1 min | TODO.md table | ❌ |

**Notes:**
- Total weekly friction: ~2 hours
- Priority 1: Email auth (gog keyring env variable)
- Priority 2: Session handoff template (just created)
- Priority 3: Prediction template (phase 2)

---

## ⚠️ Risk Assessment Template (Loop 8)

Use for every non-trivial task:

**Task:** [What]  
**Pre-Risk:** [Low/Medium/High] - [Why]  
**Post-Risk:** [Low/Medium/High] - [Actual]  
**Delta:** [If risk was misjudged]  
**Lesson:** [Next time assess differently]

---

## Active

- [ ] ID: AUTO-002
  Title: Personal Tutor - Trading Education [SYNCTEST]
  Owner: Lisa
  Risk: Low
  Done Condition: 30-day curriculum delivered mornings, tracked in Notion
  Notes: S&D, ORB, market structure lessons. Morning delivery via Discord.

- [ ] ID: AUTO-003
  Title: Research Pipeline - BGBB Content
  Owner: Lisa
  Risk: Medium
  Done Condition: Automated research → script drafts for Board Games Before Bed
  Notes: X/Reddit monitoring → research → content. Requires X API or scraping.

- [ ] ID: AUTO-005
  Title: Overnight Protocol - Self-Expanding Tasks
  Owner: Lisa
  Risk: Low
  Done Condition: 3 cron jobs (2am, 4am, 6am) active, self-expanding tasks working, morning briefings readable
  Notes: Based on @legendaryy article. Crons check todo.md, update progress-log.md, write morning brief.

- [ ] ID: AUTO-011
  Title: LifeOS - Million Dollar Digest
  Owner: Lisa
  Risk: Low
  Done Condition: Digest generation workflow runs automatically and posts/report output is logged
  Notes: Source: notion.so/LifeOS-Million-Dollar-Digest-314eed5e67c981719594d73303fe1cda. 2026-02-28 progress: workflow spec + runner added (`tasks/auto-011-million-dollar-digest/digest-workflow-spec.md`, `scripts/million-dollar-digest.sh`), first digest generated at `tasks/auto-011-million-dollar-digest/outputs/2026-02-28-million-dollar-digest.md` and logged in run-log.

---

## Completed

- [x] ID: AUTO-010
  Title: LifeOS - The Lightbulb Workflow
  Owner: Lisa
  Status: Complete
  Risk: Low
  Done Condition: Workflow documented, automated trigger path defined, and first execution run logged ✅
  Notes: Spec `tasks/auto-010-lightbulb/lightbulb-workflow-spec.md`; automation path `tasks/auto-010-lightbulb/lightbulb-automation-plan.md`; verified run on 2026-02-28 09:45 MST via `bash scripts/lightbulb-daily.sh` with observed updates in `tasks/auto-010-lightbulb/daily-summary.md` and `tasks/auto-010-lightbulb/inbox.md`.

- [x] ID: AUTO-001
  Title: "The Huddle" - Weekly Coach Automation
  Owner: Lisa
  Status: Complete
  Risk: Low
  Done Condition: Sunday morning check-in delivered via Discord, tracked in Notion ✅
  Notes: Cron Sundays 10AM live (guild 1473058960855793960 #control-center). DB 07f99572-4fc7-4c0c-b48e-0de45b01fe08. Test verified.

- [x] ID: AUTO-006
  Title: Prop Firm Intelligence
  Owner: Lisa
  Status: Complete
  Risk: Low
  Done Condition: Notion page populated with firm data ✅
  Notes: DB (276cfee9-713d-4d85-95f1-09b9e46c51a9) populated. Weekly Sundays 8AM cron live → tavily/DB update → report #control-center.

- [x] ID: OS-001
  Title: Life OS Upgrades - Auto-Retry, Dashboard, Health Checks
  Owner: Lisa
  Status: Complete ✅
  Risk: Low
  Done Condition: Health check skill implemented and running
  Notes: Healthcheck skill installed. Daily cron active (2AM, silent unless DEGRADED/FAILED). Dashboard + Backup + Healthcheck triad complete.

- [x] ID: MC-L2-001
  Title: Introduce todo.md state tracking into Mission Control
  Owner: Lisa
  Status: Complete
  Risk: Low
  Done Condition: Mission Control shows top 5 active tasks from todo.md ✅
  Notes: Created as part of Level 1 hardening.

---

## Backlog

- [ ] ID: OS-002
  Title: Trading Research Enhancements
  Owner: Lisa
  Risk: Low
  Done Condition: Research scratchpad + structured prompts implemented
  Notes: Inspired by Dexter (virattt/dexter). Research only - no trade execution.

- [ ] ID: OS-003
  Title: Digital Citadel - Identity Preservation
  Owner: Lisa
  Risk: Low
  Done Condition: SELF.md + Recovery Protocol + Backup + Journal implemented
  Notes: Inspired by sene1337/digital-citadel. Identity survival protocol.

- [ ] ID: OS-005
  Title: Multi-Agent Teams Architecture
  Owner: Lisa
  Risk: Low
  Done Condition: Trading Team fully operational
  Notes: Teams: Trading (Market+Journal+Coach), Content (Research+Script+Social), Life Ops (Huddle+Reminder+Health).

- [ ] ID: MC-L2-002
  Title: Add Approval Console (Level 2)
  Owner: Lisa
  Risk: Medium
  Done Condition: Manual approval queue visible in Mission Control

- [ ] ID: AUTO-007
  Title: Morning Magazine Pro
  Owner: Lisa
  Risk: Low
  Done Condition: Enhanced morning brief runs daily 6:30am
  Notes: Market, futures, VIX, economic calendar, sports, board games, pet industry. Posts to Discord.

- [ ] ID: AUTO-008
  Title: Trade Journal & Debrief
  Owner: Lisa
  Risk: Low
  Done Condition: Post-trade debrief system capturing wins, mistakes, rules
  Notes: Prompts after trades, saves to Notion, compounds edge over time.

- [ ] ID: AUTO-009
  Title: Idea Catcher
  Owner: Lisa
  Risk: Low
  Done Condition: Capture system for trading insights, content ideas, business thoughts
  Notes: Categories: trading, content, business, personal. Never lose an idea.
