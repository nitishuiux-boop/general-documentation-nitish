# Learnings: documentation corrections from Nitish

Newest at the bottom. One entry per correction. Each entry: date · what happened · the rule.
These override SKILL.md when they conflict.

---

- **2026-10-07** · Asked "what features exist / don't exist". Got a long Notion research page. Strong rejection.
  **Rule:** answer the literal question with the smallest output. A 2-column table was enough. No new pages unless asked.

- **2026-10-07** · Asked for features grouped. Wanted 5 clear groups: exists no issue, exists with issue, not sure, research says remove, doesn't exist.
  **Rule:** sort into the groups asked for, add a short "what it is" line, miss nothing.

- **2026-10-07** · Doc said "remove spin the wheel / RentPass / surveys / stories". Code and data showed spin and RentPass were already dead; surveys and stories were to be kept.
  **Rule:** check the source of truth (code, data) before writing. Never remove what the owner wants to keep.

- **2026-10-07** · Asked to update the main research doc. "Keep the formatting in check, do not go beyond the current format."
  **Rule:** match the existing format exactly. Smallest edit. Update every count on the page.

- **2026-10-07** · Added a 3-column layout in Notion. "It does not look good."
  **Rule:** no multi-column layouts in Notion. Use plain lists.

- **2026-10-07** · Asked for a toggle heading over a list, plus a description visible when closed.
  **Rule:** visible description goes as a grey line above the toggle heading.

- **2026-10-07** · Notion edits that renamed a toggle heading unfolded the toggle twice.
  **Rule:** after touching a toggle heading, re-fetch and check nesting. Replace the whole toggle block.

- **2026-10-08** · Persona page. Wanted: linear, scannable, no text dumps, no long bullets, airplane-manual language, evidence only for non-obvious items.
  **Rule:** same labelled parts per persona, RULE / NOTE / CAUTION callouts, evidence only where someone might question it.

- **2026-10-08** · Persona page used 5 personas from data; the spec repo had 8.
  **Rule:** when a spec repo exists, use its full list as the base. Mark each item's evidence strength instead of dropping it.
