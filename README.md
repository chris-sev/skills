# make-it-skim

Reformat and lightly edit any writing so a skimming reader still gets the full message, without changing its facts or meaning.

People do not read on screens. They scan. This skill takes finished text (an email, a doc, a post, a report, UI copy) and breaks the wall apart: short paragraphs, bullets where the text already lists something, bold on the numbers and names, a block quote for the one line that must be seen, white space between ideas. Same facts, same meaning, same order. Just readable at a skim.

It stands alone. No other skill is required to use it.

## Before and after

**Before (clean sentences, still a wall):**

> Hi team, I wanted to give everyone a quick update on where we landed with the pricing review this week. After a lot of discussion with finance and a careful look at the churn numbers from last quarter, we have decided that we are going to hold current prices through the end of the quarter and revisit in January, and in the meantime Kapehe is going to pull the retention numbers for the top twenty accounts so we can see whether the discount cohort is actually behaving differently, and if anyone has concerns about specific accounts please let me know before Friday so we can factor them in.

**After (make-it-skim, same content, formatted):**

> Hi team, a quick update on where we landed with the **pricing review** this week.
>
> After a lot of discussion with **finance** and a careful look at the **churn numbers from last quarter**, we are going to **hold current prices through the end of the quarter** and **revisit in January**.
>
> - **Kapehe** will pull the retention numbers for the **top 20 accounts**, so we can see whether the discount cohort is actually behaving differently
> - Concerns about specific accounts: please let me know **before Friday**, so we can factor them in

Nothing was added or summarized. The sentences were broken apart and tightened lightly, with the numbers, names, and the deadline bolded so a scanner lands on them. Read only the bold words and you still get the whole email.

## The research

Built on Nielsen Norman Group eyetracking research, running since 1997:

- **79% of readers scan** a new page. **16% read word by word.** (Morkes and Nielsen, 1997)
- The same content, five ways: a **scannable layout alone scored +47%** on measured usability. The facts did not change. The formatting did.
- Readers follow four scanning patterns: **F-pattern** (the failure mode a wall of text forces), **spotted** (eyes land on bold words, numbers, names, lists, block quotes), **layer-cake** (scan the headings of a longer piece, dive where relevant), and **commitment** (rare, and even committed readers do better with chunking).

## The formatting moves (short version)

1. Break the wall. Max three short sentences per paragraph, one idea each, blank line between.
2. Surface the main point. Move the line that is already there to the top, or block quote it. A light rewording is fine if it says exactly the same thing; never summarize away a fact.
3. Bullets where the text already lists something hiding in a comma chain. Numbered only when order matters.
4. Front-load every bullet with its point, in the author's words.
5. Bold anchors only: numbers, names, dates, deadlines, one key phrase per block.
6. Block quote the one line that must be seen. One per piece, at most.
7. Label the parts to help the scan, in the author's terms or a plain label you coin. A label names content already there; never invent a section and fill it. Short pieces usually need no labels.
8. Questions on their own lines, in the author's exact words.
9. White space is structure.
10. End on the author's ask if there is one, on its own line. If there is no ask, invent none.

## The tests

Every output gets three checks:

1. **Skim test:** the first line, the bold anchors, any block quote, and the first three words of every bullet carry the full message.
2. **Difference test:** every fact in the after traces to a line in the before, at the same strength, and every fact that mattered in the before is still there. A discussion is not an approval. A plan to check is not a finding.
3. **Leave-alone test:** if the original already skims well, it comes back unchanged.

## Pairs well with (optional)

If you also use a skill that cleans up the sentences themselves, run that first and make-it-skim last, because the skim pass works best on near-final text. The stack Chris uses is in the launch post. None of it is a requirement for this skill.

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
