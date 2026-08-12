---
title: "Contentful Greenfield Starter - Enterprise Blueprint"
author: "Gilberto Haro"
date: 2026-07-24
version: "1.1 current-state alignment"
status: "Active — Two-Environment Constraint Recorded"
current_phase: "00 - Baseline (Batches 00.1–00.2 approved; Batch 00.3 next)"
model_target: "10 core types"
source_format: "Markdown alignment derived from PDF blueprint"
---

# Contentful Greenfield Starter

## Enterprise Blueprint

*A print-ready operating model for content strategy, Contentful governance, migration-first modeling, frontend integration, editorial workflows, and release quality.*

| Status | Current phase | Model target |
| --- | --- | --- |
| Active — Two-Environment Constraint Recorded | 00 - Baseline; 00.1–00.2 approved | 10 core types |

> **Project Mantra: Architecture north star**
>
> Content strategy before content models. Routes before templates. UI contracts before CMS data. Static fixtures before Contentful. Validation before closeout. Documentation is part of the build.

**Prepared for:** Gilberto Haro - Web Content & Marketing Technologist  
**Version:** 1.1 current-state alignment  
**Date:** July 24, 2026  
**Research approach:** Project-source synthesis plus official Contentful, Vite, Netlify, OWASP, W3C WAI, and Google Search documentation.

# Document Control

| Item | Value |
| --- | --- |
| Document owner | Gilberto Haro |
| Project | contentful-greenfield-starter |
| Document purpose | Enterprise operating blueprint, current-state record, and printable study guide |
| Current phase | Phase 00 — Baseline + Two-Environment Setup |
| Approved work | Batch 00.1 — Repository and Project Truth; Batch 00.2 — Runtime and Contentful Tooling |
| Next planned batch | Batch 00.3 — Two-Environment Strategy Alignment + Secret Safety |
| Model target | 10 semantic content types |
| Space license | Contentful Starter — $0/month |
| Environment capacity | 2 total environments |
| Current environments | `master` (protected baseline) and `dev` (rotating sandbox) |
| Verification model | Serial clean-room verification by rebuilding the `dev` slot from protected `master` |
| Repository status | Repository/tooling repair independently verified; focused commit pending at time of alignment |
| Review cadence | At every batch closeout and before each phase transition |
| Classification | Personal project — do not include client-confidential content or real tokens |

## Approval and Change Record

| **Version** | **Date**        | **Change**                                                                                                                                                                                           | **Decision Status**       |
| ----------- | --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------- |
| 0.1         | July 23, 2026   | Greenfield direction and starter scaffold established                                                                                                                                                | Accepted                  |
| 1.0         | July 23, 2026   | Enterprise printable blueprint created as the initial governed implementation plan                                                                                                                   | Superseded                |
| 1.1         | July 24, 2026   | Repository and tooling state aligned; Starter two-environment limit incorporated; serial verification strategy adopted                                                                               | Accepted                  |
| 1.2         | August 11, 2026 | Phase 00 baseline completed; `master` + rotating `dev` environment topology finalized; secret-safety controls established; locale compatibility resolved; stale environment documentation reconciled | Accepted                  |
| 1.3         | August 11, 2026 | Phase 01 — Content Strategy + Route Contract opened; Batch 01.1 Content Strategy Foundation established as the next active workstream                                                                | **Current / In Progress** |

### Current approved direction

The project has now moved beyond its original blueprint assumptions. The operative architecture is the **two-environment model** with protected `master` and a rotating `dev` environment used for controlled serial verification—not the older persistent `master → dev → verification` topology documented in the superseded blueprint. The project remains governed by the sequence **content strategy → route contract → UI/data contracts → Contentful integration**.

**Current project state:**

```text
Phase 00 — COMPLETE
Phase 01 — ACTIVE
Batch 01.1 — Content Strategy Foundation
Contentful bootstrap migration — BLOCKED / NOT RUN
Seed content — NOT STARTED
```

The Phase 01 intake material is intended to establish mission, audiences, content pillars, route intent, CMS/code ownership, fixture requirements, SEO direction, localization, and privacy constraints before downstream modeling begins.

This makes **v1.3 the current working record** while preserving v1.2 as the approved Phase 00 closeout baseline.

## Current-State Snapshot

| Area | Current state |
| --- | --- |
| Repository identity | `contentful-greenfield-starter` |
| Package manager | `npm@10.8.3` |
| Runtime declaration | Node major `22`; detected Node `v22.2.0`, npm `10.8.3` |
| Contentful tooling | CLI package `4.0.4`; migration `5.1.0`; export `8.1.1`; import `10.0.18` |
| Contentful space | Personal Website CMS — Greenfield Starter |
| Organization | Gilberto A Haro Web Technology |
| Space ID | Recorded in private Phase 00 evidence; omitted from this shareable blueprint |
| Environments | `master` and `dev`; 2 of 2 environment capacity in use |
| Phase status | Phase 00 remains active |
| Schema status | Bootstrap migration has not been run |
| Primary blocker | None; documentation must reflect the two-environment topology before secret and environment verification work |
| Next action | Complete Batch 00.3, then verify locale, blank `master`, `dev`, and environment-safety evidence |

> **CURRENT-STATE CONTROL**
>
> The previous three-environment design (`master`, `dev`, `verification`) is superseded for this Starter space. “Verification” is now a controlled workflow state performed by rebuilding the single sandbox slot, not a permanently available third environment.

## How to Use This Document

- Use Part I to align stakeholders on purpose, scope, architecture, and success criteria.
- Use Part II as the operating roadmap and task inventory. Do not advance a phase until its gates pass.
- Use Part III when reviewing content types, fields, references, editorial behavior, and branding alignment.
- Use Part IV to implement the secure frontend and server boundary after the model and contracts are stable.
- Use Part V for study, review, knowledge checks, and blog planning.
- Update the repository truth surfaces after every approved batch so this PDF does not become the only source of truth.

> **CONTROL: Important boundary**

> This document is a comprehensive plan, not evidence that a phase has passed. Only recorded verification in the repository can close a phase.

# Table of Contents

Use this document map to navigate the printed blueprint. The PDF bookmarks and heading structure provide additional navigation in compatible readers.

| Section | Purpose |
| --- | --- |
| 1. Executive Summary | Project direction, outcomes, and enterprise definition of success. |
| 2. Project Charter | Vision, objectives, scope, stakeholders, and accountability. |
| 3. Architecture Principles | Decision framework and non-negotiable system boundaries. |
| 4. Environment, Migration, and Replication | two-environment master/dev topology, serial clean-room verification,<br>migrations, snapshots, and import/export limitations. |
| 5. Brand, Content, and Route System | Brand direction, content pillars, route ownership, SEO intent, and<br>responsive behavior. |
| 6. Content Model v1 | Ten core types, fields, references, field governance, and<br>deferred decisions. |
| 7. Repository Operating System | Truth surfaces, closeout rules, and context-drift prevention. |
| 8. Frontend, API, and Adapter Architecture | Secure delivery boundary, API roles, contracts, and secret<br>controls. |
| 9. Editorial Workflow | Roles, authoring checklist, preview, and supporting CMS<br>resources. |
| 10. Quality, Accessibility, SEO, and Release | Quality gates, WCAG baseline, sitemap, structured data, and<br>release controls. |
| 11. Enterprise Risk Register | Risks, impact, likelihood, mitigations, and review cadence. |
| 12. Detailed Phase Roadmap | Complete objectives, tasks, deliverables, gates, and study for<br>Phases 00-09. |
| 13. Work Packages and First 30 Days | First commits, monthly cadence, and day-one commands. |
| 14. Checklists and Templates | Content type, migration, import/export, and route release<br>checklists. |
| 15. Study Guide | Eight-module learning plan, knowledge check, and answer key. |
| 16. Blog Development Backlog | Sixty-plus article ideas grouped by implementation theme. |
| 17. Glossary | CMS, Contentful, frontend, governance, and release terminology. |
| 18. Research Library | Official technical sources and project-source inventory. |
| 19. Immediate Action Plan | Phase 00 commands, files to update, and final definition of<br>success. |

# 1. Executive Summary

The `contentful-greenfield-starter` project establishes a small but enterprise-disciplined Contentful foundation for a personal portfolio website. The intent is not to build a generic page builder or mirror the frontend component tree inside the CMS. The intent is to create a semantic content platform that can reliably support personal positioning, projects and case studies, writing, experience, skills, navigation, SEO, and editorial preview while preserving strong frontend contracts.

The current Contentful Starter space supports two environments total. Those slots are already occupied by `master` and `dev`. The project therefore uses a **two-environment serial verification strategy**:

1. `master` remains the protected blank baseline until an approved release strategy changes its role.
2. `dev` is the only sandbox slot and is used for migration development and model review.
3. Before representative seed content is added, the approved `dev` model is exported and checksummed.
4. With explicit approval and complete recovery evidence, `dev` is deleted and recreated from protected `master`.
5. The model-only snapshot is imported into the fresh `dev`, then compared against the approved model contract.
