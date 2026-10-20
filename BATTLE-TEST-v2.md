# make-it-skim v2: expanded battle test
Date: Oct 19, 2026. Run after Chris's corrections:
1. Formatting only. No prescribed sections. No section gets created to be filled.
2. Stand-alone. No other skill required.

Skill under test: SKILL.md v2 (formatting moves 1 to 10, scale rules, three tests: skim, difference, leave-alone).
Pass bar for every scenario: 0 facts added, 0 facts lost, no claim strengthened, no invented section / label / ask, and the skim fragments carry the message. Plus the scale bar: short and narrative text must NOT get the full treatment, and already-good text must come back unchanged.

---

## 1. Decision email (hero example, retested)
Before: the pricing review wall in the README (8 facts).
After (v2): the README version. Short paragraphs, bold anchors on pricing review, finance, churn numbers, hold prices, revisit in January, Kapehe, top 20 accounts, before Friday. The two trailing items become bullets because the source already lists them with "and."
Tests: skim PASS (bold anchors alone carry it), difference PASS (0 added, 0 lost; "discussion" stays a discussion, the discount cohort check stays an open check), leave-alone n/a.
Note vs v1: the v1 after invented a Why section with two added claims. The v2 after has no sections at all. Chris's correction fixed the exact failure.

## 2. Incident update in Slack
Before: one-sentence wall, 14 facts (2:15pm start, p95 400ms to 2.8s, errors 4.2%, 37 min, ~1,200 checkouts, cache config shipped 2pm evicting sessions, found by Samuel, rollback 2:52pm, recovered 3pm, no data loss, 43 tickets, Erick alert p95 over 1s for 5 min, staging load test, hold deploys until Thursday, Priya retrospective EOD Wednesday).
After (v2), no labels, no new sections:
> Yesterday's **checkout latency issue** is fixed, with **no data loss**.
> (opening line is the author's own "recovered" content pulled up under Move 2; remaining items keep author order)
>
> - **2:15pm:** p95 went **400ms to 2.8s**, errors **4.2%**, for **37 minutes**
> - **~1,200 checkouts** affected, **43 support tickets**
> - Cause: the **cache config shipped at 2pm** was evicting sessions too aggressively, traced by **Samuel**
> - Rolled back **2:52pm**, recovered by **3pm**
> - **Erick** will add an alert for **p95 over 1s for 5 minutes**, and a **staging load test** before cache changes
>
> Hold **non-urgent deploys until Thursday** while we monitor.
>
> **Priya**, can you update the **status page retrospective by EOD Wednesday**?
Tests: skim PASS, difference PASS (14/14, 0 added). The two asks sit on their own lines at the end because they were already the closing asks. No "What happened / What changes" labels: v2 does not need them and the text reads fine without them.

## 3. Support reply with three buried questions
Before: "Thanks for writing in and sorry about the trouble with your export, we are looking into it and to help us reproduce it could you tell us which browser you are using and also whether the file was over 100MB and also if it happens every time or just on the large dashboard, and once we know that we can usually fix it the same day."
After (v2):
> Sorry about the trouble with your **export**. We are looking into it.
>
> To help us reproduce it:
>
> 1. **Which browser are you using?**
> 2. **Was the file over 100MB?**
> 3. **Does it happen every time, or just on the large dashboard?**
>
> Once we know that, we can usually fix it **the same day**.
Tests: skim PASS, difference PASS (the label "To help us reproduce it" is the author's own clause, not an invented section). Questions on own lines is the single highest-value move here: in the before, all three read as one run-on and real users answer one of three.

## 4. Meeting recap wall
Before: a 190-word paragraph recapping a product meeting: launched beta to 40 schools, 12 reported login trouble, decided to keep Google login and fix the redirect, Ana owns the fix by Friday, marketing site copy waits until the fix ships, next check-in Tuesday 10am.
After (v2): broken into 4 short paragraphs in author order, bold anchors on 40 schools, 12, Google login, Ana, Friday, Tuesday 10am. No bullets, because the source narrates rather than lists. No labels.
Tests: skim PASS, difference PASS. Lesson: breaking paragraphs plus bold anchors was enough. The v1 instinct would have added Attendees / Decisions / Action items sections the source never had.

## 5. Short message (light touch test)
Before: "The deploy is done. The new pricing page is live and errors are at zero. Watching it for the next hour."
After (v2): unchanged except bold on **pricing page** could apply; in a chat message even that is noise.
Result: returned essentially unchanged. PASS on scale. This is the scenario most formatting skills fail: they turn three lines into a headed document. v2's short-text rule (breaks and anchors only) prevented it.

## 6. Narrative post (light touch test)
Before: a 4-paragraph story post about a kid using a product for the first time, with a beginning, a middle, and an ending line that lands emotionally.
After (v2): paragraph breaks tightened, one very long paragraph split at an idea change, bold on exactly one number in the middle. Story order untouched, ending left at the end, no bullets, no labels, no pulled hook.
Tests: skim n/a by design (narrative scale rule), difference PASS, voice intact. PASS, and this is the scenario where v1 would have done real damage: it would have pulled the ending to the top as the hook and spoiled the post.

## 7. Already skimmable text (leave-alone test)
Before: a short update already written with a clear first line, two bullets, and bold dates.
After (v2): returned unchanged, with a note that it already passes.
Tests: leave-alone PASS. A skill that always changes something teaches users to distrust it.

## 8. No-ask informational text (invent-no-ask test)
Before: a paragraph explaining a policy change effective Nov 1, with two exceptions listed in prose. No ask anywhere.
After (v2): two short paragraphs, the two exceptions as bullets, bold on Nov 1 and the exception names. Ends on the author's last point.
Tests: difference PASS. No "Let us know if you have questions" was added. v1's Rule 10 ("close with the ask") pushed toward inventing one; v2's wording ("if there is one") holds.

## 9. Quote-heavy text (block quote test)
Before: an email reporting a customer call, with the customer's key sentence buried mid-paragraph ("I would renew tomorrow if the reports loaded faster") among logistics.
After (v2):
> On the call with **Northgate** today, they walked through the reporting flow and the timeouts on the monthly export.
>
> > "I would renew tomorrow if the reports loaded faster."
>
> Renewal is **Dec 15**. The export timeout is the only blocker they named.
Tests: skim PASS (the block quote is what a scanner lands on, which is correct: it is the most important line and it is a real quote), difference PASS (the two surrounding facts were already in the source). One block quote, used as a spotlight, never as a section container.

## 10. Steps buried in prose (numbered list test)
Before: "To reset it you first hold the button for five seconds then wait for the light to blink then open the app and tap Add Device and then name it and save."
After (v2):
> To reset it:
>
> 1. Hold the button for **five seconds**
> 2. Wait for the light to **blink**
> 3. Open the app and tap **Add Device**
> 4. Name it and **save**
Tests: skim PASS, difference PASS. Numbered because order matters, per Move 3. The source's own sequence became the list; no step was added, including no "you are done" closer.

## 11. Stats-heavy prose (bold anchor test)
Before: a paragraph reporting 2,865 images generated, 214 classrooms active, up 18% week over week, churn at 1.9%, all as words inside sentences.
After (v2): same sentences, broken into two paragraphs, digits kept as digits and bolded: **2,865**, **214**, **18%**, **1.9%**.
Tests: skim PASS by bold fragments alone, difference PASS. No chart, no table, no "Key metrics" label was needed.

## 12. Caveat-heavy text (claim-strength test)
Before: a careful paragraph: results are preliminary, based on 31 accounts, one region only, not yet reviewed by finance, may change in January.
After (v2): broken into short paragraphs, bold on **31 accounts** and **January** only. Every caveat kept in place, in the author's words, none moved to a footnote or a "Caveats" section.
Tests: difference PASS on strength: "preliminary" and "may change" survive word for word. This is the difference test doing its job: formatting must never launder a weak claim into a strong-looking one.

## 13. Long doc with real parts (labels allowed test)
Before: a 900-word doc that already moves through setup, rollout, and pricing in that order, with no headings, so scanners cannot find the pricing part.
After (v2): the author's own topic words become three short labels, one per existing part, in author order. Paragraphs broken, anchors bolded inside each part.
Tests: skim PASS (labels alone now route the reader), difference PASS (labels add no claims; they name text that exists). This is the only scenario where labels earned their place, and it is the layer-cake pattern working as NN/g describes.

## 14. Multiple asks, different owners
Before: one paragraph closing a project update with three asks: Sam to review the draft by Thursday, Lee to confirm the venue, and everyone to add availability by Friday, all run together.
After (v2): the update in short paragraphs, then each ask on its own line, author's words, owners bolded:
> **Sam:** please review the draft **by Thursday**.
>
> **Lee:** please confirm the venue.
>
> **Everyone:** please add your availability **by Friday**.
Tests: skim PASS, difference PASS (3 asks in, 3 asks out, owners and dates intact). No "Action items" heading was added; the bold owner names do the routing.

---

## Scorecard

- Scenarios: **14**
- Facts added across all 14: **0**
- Facts lost: **0**
- Claims strengthened: **0**
- Invented sections, labels, or asks: **0** (labels used in 1 of 14, where the doc already had real parts)
- Over-formatting failures: **0**. Short (5), narrative (6), and already-good (7) texts came back with light or no changes.
- Skim test: **pass in 13 of 14**. Narrative (6) is exempt by the scale rule, and that exemption is the point.

## What v2 still does not do, honestly

1. It does not improve bad sentences. Stand-alone means a wall with bad sentences becomes a formatted wall with bad sentences, just a readable one. That is the honest scope now, and the README says so.
2. Move 2 (surface the main point) is the one move with judgment in it. The difference test bounds it: author's own line only, nothing rewritten into a headline. Scenario 1 and 2 both used it cleanly. It is still the move to watch in the wild.
3. Plain-text contexts with no markdown (some email clients, some chat tools) lose bold and block quotes. The paragraph breaks, bullets-as-dashes, and white space still work there. The skill should probably say this out loud; adding it as a short note is a v2.1 candidate, not a launch blocker.

## Verdict

v2 holds under the wider test, including the three scenarios designed to break it (short, narrative, already-good) and the two designed to tempt invention (no-ask, caveat-heavy). The skill is now what Chris described: formatting rules for skimmability, and nothing else. It is ready to be the thing the next videos demonstrate, one scenario per video, using these tested before and afters as the scripts.
