# make-it-skim

Structure any writing so a skimming reader still gets the full message.

People do not read on screens. They scan. This skill restructures anything your agent writes (emails, docs, posts, reports, UI copy) so the skimmer gets the point, the facts, and the ask anyway.

## Before and after

**Before (clean sentences, still a wall):**

> Hi team, I wanted to give everyone a quick update on where we landed with the pricing review this week. After a lot of discussion with finance and a careful look at the churn numbers from last quarter, we have decided that we are going to hold current prices through the end of the quarter and revisit in January, and in the meantime Kapehe is going to pull the retention numbers for the top twenty accounts so we can see whether the discount cohort is actually behaving differently, and if anyone has concerns about specific accounts please let me know before Friday so we can factor them in.

**After (make-it-skim):**

> **Decision: prices stay as they are through the end of the quarter.** We revisit in January.
>
> Why:
> - Finance signed off after reviewing last quarter's churn numbers.
> - No evidence yet that discounts change retention.
>
> Next steps:
> - **Kapehe** pulls retention numbers for the **top 20 accounts** this week.
> - Concerns about a specific account: send them to me **before Friday**.

Same facts. The second version survives a skim.

## Why: the research

Built on Nielsen Norman Group eyetracking research, running since 1997:

- **79% of readers scan** a new page. **16% read word by word.** (Morkes and Nielsen, 1997)
- The same content, five ways: **concise +58%**, **scannable layout +47%**, **objective language +27%** on measured usability. **All three: +124%.**
- Readers follow four scanning patterns: **F-pattern** (the failure mode a wall of text forces), **spotted** (eyes land on bold words, numbers, names), **layer-cake** (scan the headings, dive where relevant; the goal), and **commitment** (rare, and even committed readers do better with chunking).

## Where it fits

The AI writing stack has three layers:

1. **unslop** cleans the words.
2. **humanizer** fixes the voice.
3. **make-it-skim** fixes the structure.

The first two make AI writing sound human. This one makes it readable by one.

## The rules (short version)

1. Hook line first. The point stands alone at the top.
2. One idea per line or paragraph.
3. Signpost every section with a descriptive heading or bold lead.
4. Lists over prose.
5. Front-load every bullet. Never repeat bullet openings.
6. Bold anchors only: numbers, names, dates, the key phrase.
7. Numbers beat adjectives.
8. White space is structure.
9. Questions get their own lines.
10. The ask closes, on its own line.

## The Skim Test

Every output ends with two checks:

1. **Layer-cake test:** the headings alone tell the whole story.
2. **Skim test:** the hook, the bold anchors, the first three words of every bullet, and the closing line carry the full message.

If the fragments do not carry it, the skill rewrites until they do.

## Install

```bash
npx skills add chris-sev/skills --skill make-it-skim
```

Works with Claude Code, Codex, Cursor, and other agents that load SKILL.md files. Or copy `skills/make-it-skim/SKILL.md` into your agent's skills folder directly.

## Sources

- Nielsen Norman Group, "How Users Read on the Web" (1997)
- Nielsen Norman Group, "Concise, SCANNABLE, and Objective: How to Write for the Web"
- Nielsen Norman Group, "Text Scanning Patterns: Eyetracking Evidence"
- Nielsen Norman Group, "The Layer-Cake Pattern of Scanning Content on the Web"
- Nielsen Norman Group, "F-Shaped Pattern of Reading: Misunderstood, But Still Relevant"
- Nielsen Norman Group, "How People Read Online: New and Old Findings"

Full links are in the SKILL.md.

## License

MIT
