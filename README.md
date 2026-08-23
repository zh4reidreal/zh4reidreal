<div align="center">

# ZH4REID

Node.js developer building Discord automation
and operational systems for communities.

[github.com/zh4reidreal](https://github.com/zh4reidreal)

</div>

---

I design and ship practical Discord systems — moderation pipelines, permission control, ticket workflows, and config-driven bots that keep servers running.

The work is Node.js first. Small surface area. Clear boundaries. Systems that operators can actually use.

---

## About

I work on Discord infrastructure for live communities.

Most of what I build sits at the intersection of automation and operations: member onboarding, word filters and penalty flows, interactive role management, support tickets, and lightweight persistence.

I prefer systems that are configuration-driven rather than hard-coded, with permission checks before every privileged action and a log trail after.

---

## Focus

| Area | What I build |
| --- | --- |
| Discord Automation | Bots that carry the operational load of a server — replies, moderation, onboarding, support |
| Permission Systems | Role control with hierarchy checks, authorized operators, and audit logs |
| Node.js Systems | JavaScript services with discord.js, Express, and simple durable storage |

---

## Stack

Only what the running systems actually use.

| Layer | |
| --- | --- |
| Language | JavaScript |
| Runtime | Node.js |
| Platform | discord.js |
| HTTP | Express |
| Data | JSON · filesystem |
| Tooling | Git · GitHub |

---

## Selected Work

Source for these systems is private. They are the core of my current engineering work.

| System | Role | Stack | Status |
| --- | --- | --- | --- |
| **99V APEX** | Server operations bot. Auto-role and welcome flow, word filter with penalty points and timeouts, auto-replies, user query, ticket channels, message-based wallet. Express keep-alive. | Node.js · discord.js · Express | Private |
| **Yetki** | Interactive permission panel. Authorized operators grant or revoke roles through buttons and select menus, with hierarchy validation, duplicate-role guards, and channel logging. | Node.js · discord.js | Private |

---

## System Map

```text
99V APEX
  member join   →  unverified role + welcome
  message       →  filter / auto-reply / wallet
  command       →  profile query · ticket panel
  ticket        →  modal → private channel

YETKI
  operator      →  authorized role check
  panel         →  grant / revoke
  mutate        →  hierarchy check → log
```

---

## Approach

- Prefer configuration over scattered constants.
- Check permissions before mutating state.
- Log privileged actions.
- Keep the runtime small enough to reason about.
- Ship something a server can run today, then tighten the structure.

---

## Now

- Discord automation for community operations
- Permission and role-control flows
- Tightening this profile and how the work is presented

---

## Direction

- Split monolithic bot files into clearer modules
- Move secrets out of the repository
- Give internal tools public, documented counterparts
- Strengthen persistence beyond flat JSON where it matters

---

## Contact

GitHub is the right place to reach me.

**[zh4reidreal](https://github.com/zh4reidreal)**

---

<div align="center">

<sub>zh4reid · Node.js · Discord systems</sub>

</div>
