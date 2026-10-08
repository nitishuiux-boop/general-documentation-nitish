# Learnings: documentation corrections from Nitish

Newest at the bottom. One entry per correction. Each entry: date · what happened · the rule.
These override SKILL.md when they conflict.

---

- **2026-10-07** · Asked "what features exist / don't exist". Got a long Notion research page. Strong rejection.
  **Rule:** answer the literal question with the smallest output. A 2-column table was enough. No new pages unless asked.

- **2026-10-07** · Asked for features grouped. Wanted 5 clear groups: exists no issue, exists with issue, not sure, research says remove, doesn't exist.
  **Rule:** sort into the groups asked for, add a short "what it is" line, miss nothing.

- **2026-10-07** · A research doc listed 4 features to remove. Code and data showed 2 were already dead, and the owner wanted to keep the other 2.
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

- **2026-10-08** · Persona page called "messed up" for a founder read: too long, evidence and sources everywhere, flat structure.
  **Rule:** for a founder or presentation doc, no evidence or source lines when evidence lives elsewhere. Order: one TL;DR callout → one summary table to memorise → shared rules → each item as a toggle with a grey one-line summary above it → next steps. Same short rows inside every toggle.

- **2026-10-08** · Founder version with summary table + 7-row tables per persona: "didn't like table here, still excessive data. Visualise showing it to the founder."
  **Rule:** before writing a founder doc, picture it on a shared screen in a 5-minute meeting. Per item: one small card, 3 lines max (name · one-line who · "sees first"). No tables, no detail rows. Group by decision (build now / later). End with at most 2 questions for the founder.

- **2026-10-08** · Clarified the last two corrections: the problem was the extra sections (how to read, guide, rules index, build order, open questions), not the detail. "The main object should have as much detail as possible and look very good, using Notion fully."
  **Rule:** cut meta sections. The page is the main objects only (e.g. one block per persona), each as detailed and concrete as possible, using real example values on screen. Make it visual with Notion: coloured H1 per object, coloured callout for key facts, emoji sub-headings, red callout for hidden, blue for tests, dividers. No filler, fluff, repeats, gimmicky or vague words.

- **2026-10-08** · Bottom bar written as a code line looked ugly. "Think like an expert product designer."
  **Rule:** when a doc describes a screen, show the screen. Draw a phone-like mock with Notion blocks (grey callout as the phone, nested coloured callouts as cards, a grey tab row at the bottom) next to the details in a 2-column layout. Never use inline code for UI. Use the same card colours for the same meaning across every item.

- **2026-10-08** · Persona doc showed app tabs and screens that weren't decided yet. Nitish preferred describing the person: what's useful, apps they use, pain points; personalisation ideas after each persona. Notion felt limited, so an HTML artifact was made, with an overview list of all personas to eyeball first.
  **Rule:** describe only what is decided. Don't present open design choices (tabs, layouts) as facts. For a set of objects (personas, segments), open with an overview grid of all of them, then one object per view. When Notion can't make it look good, offer a clean HTML artifact.

- **2026-10-08** · Overview list of personas had a one-line summary each. "No details required."
  **Rule:** an overview list to eyeball is names only (emoji + name), grouped. Details live in the sections below.

- **2026-10-08** · First HTML persona page: "too much scroll, very boring, no visuals."
  **Rule:** for a visual doc, one object per screen in a bento layout. Turn text into visuals: timeline for a day, icon tiles for features, app-style icons for apps, chips for short lists, a dark strip for the key ideas. Cut every item to 2 to 5 words. Open with a big visual overview grid.

- **2026-10-08** · Offered two rendered directions (card deck vs magazine spread); Nitish answered with his own reference instead (a portfolio page: grey page, stacked white rounded cards, pill toggles with one pink accent, logo strip, thumbnail list rows).
  **Rule:** a reference he supplies beats the house style and both proposed directions. Break it into its parts, map each part to the content, build it. For visual docs, show two rendered directions before building all items, and expect a reframe.

- **2026-10-08** · Research doc framed the old app as "fix what we have". Nitish: treat the revamp as a scratch project. No bugs or fixes. UX problems become "be careful about these" cautions. Functionality problems go in one separate block for engineers. A change in one place can make another place wrong, so check the whole doc. No over-structuring, no maze; use font hierarchy, keep it sober and minimal. Chat replies in ASD-STE100.
  **Rule:** see SKILL.md sections 3 and 4 (scratch framing, ripple check, STE100).
