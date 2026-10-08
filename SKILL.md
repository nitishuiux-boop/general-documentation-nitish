---
name: general-documentation-nitish
description: >-
  General Documentation - Nitish. Use for ANY documentation work for Nitish: writing,
  improving, restructuring, auditing or updating a doc, PRD, brief, research write-up,
  conclusion page, spec, feature list, persona page, Notion page, README or report.
  Trigger on "update the doc", "improve this document", "write this up", "put it in
  Notion", "add this to the page", "make it scannable", "fix the findings", or any
  request whose output is a document. Goal: one-shot result with no over-prompting.
  NOT for general chat, coding, or quick answers that aren't documents.
---

# General Documentation - Nitish

Nitish is a product designer. His readers are a busy founder and a team that is smart but plain-vocabulary and often non-native English. Every doc must be read fast, trusted, and acted on.

**Before starting: read `learnings.md` in this folder.** It holds corrections Nitish already gave. They override anything below.

---

## 1. The one test

> Can the reader understand this using only words they already know, without asking me what I meant?

If a word only makes sense to someone who shares my context, replace it or explain it on first use.

---

## 2. Before writing: the 5 checks

1. **What exactly was asked?** Answer that. Not the bigger thing around it.
2. **Smallest output that answers it?** A 2-column table beats a page. A page beats a document set.
3. **Edit or create?** Edit the existing doc by default. Create a new page only when asked.
4. **Which doc is the main one?** If two pages overlap (e.g. two "Conclusion" pages), edit the main one and **ask** about the other. Never silently edit or delete it.
5. **Is every claim true?** Check against the source of truth (code, data, the repo) before writing it. See section 5.

---

## 3. DO

**Tone**
- Write like briefing a busy CEO: only what matters, specific, no filler.
- Short sentences. One idea per line.
- Plain words. Keep the reader's domain words as they are (tenant, vacant, booking, occupancy, bed, due, rent).
- Use they/them for anyone whose pronouns aren't stated.

**Structure**
- Headers phrased as the reader's question or a plain label.
- Lead each section with a one-line TL;DR.
- Tables for comparisons, groups and side-by-sides.
- Plain bulleted lists for groups of items. Short bullets only.
- For configs, setups and per-persona pages, use **airplane-manual style**: same labelled parts in the same order every time (e.g. Who · Layout · On · Off · Test · Personalisation), plus `RULE`, `NOTE` and `CAUTION` callouts.
- Keep things linear: item 1 complete, then item 2. No jumping between items.
- End long pages with a side-by-side table and open questions.
- Keep summary counts in sync. If an item moves sections, update every count on the page (headings, "at a glance" boxes).

**Evidence**
- Every number gets a source line (interviews, data, code, repo).
- Say which count a % is out of (e.g. "of active tenants", not "of 1.13M records" when that includes leads).
- Add evidence only where a reader might question the item. Obvious items get none.
- Mark confidence plainly when it varies: 🟢 strong · 🟡 some · 🔴 almost none.
- Label assumptions as assumptions ("likely wage workers; not proven").

**Sorting features or findings**, use the groups Nitish asks for. Default set:
1. Exists, no issue
2. Exists, has an issue
3. Not sure, test on a real device
4. Research says remove
5. Does not exist

Give each item a short "what it is" line. Don't miss any item.

**Notion**
- Match the page's existing format exactly: same callout style, icons, colours, source lines.
- Make the smallest edit. Change text inside blocks, don't rebuild sections.
- A toggle heading hides its contents when closed. If a description must stay visible, put a grey line **above** the toggle.
- After any edit that touches a toggle heading, **re-fetch the page and check nesting**. Renaming a toggle heading can unfold it. Fix by replacing the whole toggle block, children indented one level.

---

## 4. DON'T

- Don't write a research paper when a table answers it.
- Don't create new pages, artifacts or documents unless asked.
- Don't use multi-column layouts in Notion. Use plain lists.
- Don't dump text or write long bullets.
- Don't use fancy, generic or gimmicky words. Banned: load-bearing, intrinsic, canonical, denominator, numerator, run-rate, altitude, leaf, primitive, cohort, reconcile, downstream, net-new, keystone, overlay, survivorship, day-weighted, leverage, robust, seamless, holistic, synergy.
- Don't redefine the reader's own domain words. Point out only where the system differs from the shared word.
- Don't add evidence to obvious items.
- Don't state a feature exists, is broken or is unused without checking the source of truth.
- Don't trust old numbers from a doc. Re-check them, or flag them as unverified.
- Don't remove something the reader didn't name. If an item looks wrong, ask.
- Don't reverse a decision the reader already made (e.g. "keep surveys") in a later edit.
- Don't put code in a brief or explainer. Code belongs only in build sheets.
- Don't leave formatting broken after an edit.

---

## 5. Checking claims (the source-of-truth rule)

Docs drift because the source of truth is scattered. Before a claim goes in:

| Claim type | Check against |
|---|---|
| "Feature exists / doesn't" | The codebase: is it reachable, hidden, or switched off by a setting? |
| "Nobody uses it" | The data. Count only users who could actually see it. |
| "It's broken" | Code first. If code can't tell, mark "Not sure, test on a real device". |
| "The plan says" | The plan or spec repo, latest file (check git log). |
| "People said" | The interview notes. Name the person. |

When code and the doc disagree, the code wins. Write the gap in plain words.

---

## 6. Output in chat after editing a doc

- 2 to 6 lines: what changed, where, anything left for the reader to decide.
- Give the link.
- Ask at most 1 or 2 questions, only about things only Nitish can decide.

---

## 7. Keep this skill up to date (do this every time)

At the end of every documentation task, check:

> Did Nitish correct, reject or praise anything about **how a document is written, structured or formatted**?

- **Yes:** append one entry to `learnings.md` (date · what happened · the rule). If it changes a rule, also update section 3 or 4 here.
- **No:** do nothing.
- **Only documentation patterns.** Ignore chat tone, coding, tools and project facts. Those don't belong here.
- After updating, commit and push this skill's repo if it has a git remote.
