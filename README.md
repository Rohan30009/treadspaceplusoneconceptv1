# Treadspace +1 | Adaptive 120-day employee ramp

An interactive, front-end-only P0 concept demonstration based on the provided Treadspace +1 screenshots. The prototype illustrates **one coordinated employee experience** from joining through meaningful work, review, targeted learning, support, and broader ownership.

## Open the demo

**Easiest:** open `Treadspace_Plus1_Interactive_Demo.html` from the download (a standalone version is provided alongside this ZIP). It contains its styling, JavaScript, example content, and illustrative employee portrait. It runs offline in a modern browser.

**This repository / GitHub Pages:** open `index.html`, or upload all the files and folders in this ZIP to your GitHub repository. In GitHub, select **Settings → Pages → Deploy from a branch → main → /(root)**. GitHub Pages will then serve `index.html`. No installation, build tools, API keys or dependencies are required.

## Navigation

1. **Role switch** at top right: Employee (Ranvijay Singh), Manager (Aditi Rao), Human Buddy (Karan Mehta). Changing roles **does not change the day**.
2. **Day selector** in the milestone line and its tabs: Days 1, 2, 5, 14, 30, 31, 60, 90 and 120. Changing days preserves the selected role.
3. **Journey explorer** in the left sidebar or the top toolbar opens a **9 × 3 matrix**. Pick any day/role combination directly.
4. **Day 31 scenario** switch: Completed versus Needs support. The corresponding Employee, Manager and Buddy content changes. For an instructive demo, begin with Manager Day 30, then Manager Day 31 (Needs support), then Buddy Day 31.
5. **Sidebar sections** open learning, tasks, competencies, milestones, people, team overview, interventions, analytics, coaching notes and calendar tools as appropriate to the current role.
6. **Click buttons and cards** to access task briefs, learning content, supporting evidence, manager decisions, buddy coaching guides and forms. All forms record visibly to the current browser's local storage only.

## Demonstrable flows

- Day 1: HR documentation, workplace policies, IT access, team introduction and clear expectations. Administrative tasks do not increase proficiency.
- Day 2: customer context, product understanding and a real-work-adjacent architecture exercise.
- Day 5: approved repository overview, sandbox inference service, testing and initial demonstration.
- Day 14: first submission, reviewer feedback about p95 latency, targeted learning, then a better attempt.
- Day 30: a bounded real engineering contribution suggested by AI and approved by the manager, with normal testing/review controls.
- Day 31 success: validated work evidence leads to three next-task recommendations, manager authorisation and additional responsibility.
- Day 31 blocked: recognise completed work, identify possible gaps, offer focused buddy support, document the next independent step and schedule manager re-review.
- Days 60/90/120: broaden scoped autonomy, review actual impact, and transition to ordinary professional development.
- Learning library: opening a guide shows its purpose, expected learning and an action-oriented application sequence. Add to plan and mark reviewed.
- eBuddy: context-aware **scripted example responses** for the questions in the interface; no real LLM is called.
- Communications: role-targeted, local simulated messages and notes appear in the recipient role's shared-updates card.
- Notifications and activity history reflect actions taken in the demo.
- All changes can be cleared using **Reset demo state** at the page footer.

## Project structure

```
index.html        Website entry point
styles.css        Design system, layout and responsive rules
data.js           Fictional people, tasks, competency data, resources and story content
app.js            Rendering, role/day navigation, interactions and local demo persistence
assets/           Illustrative employee avatar cropped from a supplied concept screenshot
README.md         This guide
```

## P0 intent and deliberate limits

This is a realistic **product behaviour demonstration**, not a production application. No real accounts, database, Jira, GitHub, Azure DevOps, calendar, SMS/email, learning-management system or LLM are connected. Workflow actions are simulated and saved in the current browser using `localStorage`.

The proposed product logic deliberately puts final authority with human managers, restricts the human buddy to authorised support context, and treats AI-proposed competency changes as provisional pending source review and validation. The sample scores and work outcomes are placeholders, not actual assessments.

The core proposed P0 is not to replicate an LMS or a task manager. It uses initial competency evidence and organisation-defined role expectations to organise relevant learning and meaningful existing work, then adapts from reviewed work results. Real integrations, content governance, permission enforcement, scoring calibration and employer validation would be separate engineering and discovery workstreams.
