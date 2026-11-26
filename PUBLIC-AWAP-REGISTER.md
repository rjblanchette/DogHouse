# Public AWAP Register

**Register status:** ACTIVE — first entry filed 21.08.2026.

---

## 1. Purpose

This public-facing register records, for each published article, the
existence and location of its public AWAP (`AWAP-PUBLIC-<slug>.md`) and
a link back to where it was published.

The controlling closure record for each article remains in the private
canonical repository. This register is a transparency surface and does
not create or extend authorship authority.

## 2. Record model

```text
PublicAWAPRecord {
    article_slug
    work_title
    source_project              -- e.g. "SubStack"
    dog_reference                -- reference only, not the DOG itself
    closure_date                 -- date the internal AWAP closed
    published_date                -- date published to SubStack
    published_url
    public_awap_ref               -- AWAP-PUBLIC-<slug>.md in this repo
    lid_encoding_status           -- Pending / Encoded / Not Submitted
}
```

## 3. Non-authority rule

```text
entry in this register        ⇏  authorship authority
publication count              ⇏  closure completeness
presence here                  ⇏  the canonical AWAP itself
```

## 4. Register

| article_slug | work_title | published_url | closure_date | public_awap_ref | status |
|---|---|---|---|---|---|
| why-i-keep-a-record | Why I Keep a Record When I Work With AI | https://rjblanchette.substack.com/p/why-i-keep-a-record-when-i-work-with | 2026-08-21 | `AWAP-PUBLIC-why-i-keep-a-record.md` | **Published 21.08.2026** |
| surplus-after-attribution | Surplus After Attribution | https://rjblanchette.substack.com/p/surplus-after-attribution | 2026-09-05 | `AWAP-PUBLIC-surplus-after-attribution.md` | **Published 05.09.2026** |
| traceability-is-not-authority | Traceability Is Not Authority | https://rjblanchette.substack.com/p/traceability-is-not-authority | 2026-09-15 | `AWAP-PUBLIC-traceability-is-not-authority.md` | **Published 15.09.2026** |
| can-a-machine-describe-feeling-without-feeling-anything | Can a Machine Describe Feeling Without Feeling Anything? (Essay 1 of 9 — *What Does It Mean to Feel?*) | https://rjblanchette.substack.com/p/can-a-machine-describe-feeling-without | 2026-11-10 | `series/what-does-it-mean-to-feel-consciousness-conscience-and-the-possibility-of-artificial-experience/README.md` | **Published 10.11.2026** |
| authority-scarcity | Authority Scarcity: The Constitutional Challenge of the AI Age | https://rjblanchette.substack.com/p/authority-scarcity | 2026-11-22 | `AWAP-PUBLIC-authority-scarcity.md` | **Published 22.11.2026** |
| the-human-who-cannot-respond | The Human Who Cannot Respond (Essay 2 of 9 — *What Does It Mean to Feel?*) | https://rjblanchette.substack.com/p/the-human-who-cannot-respond | 2026-11-10 | `series/what-does-it-mean-to-feel-consciousness-conscience-and-the-possibility-of-artificial-experience/README.md` | **Published 13.11.2026** |
| if-i-replace-your-brain-are-you-still | If I Replace Your Brain, Are You Still There? (Essay 3 of 9 — *What Does It Mean to Feel?*) | https://rjblanchette.substack.com/p/if-i-replace-your-brain-are-you-still | 2026-11-10 | `series/what-does-it-mean-to-feel-consciousness-conscience-and-the-possibility-of-artificial-experience/README.md` | **Published 16.11.2026** |
| i-remember-my-wife-but-do-i-feel | I Remember My Wife. But Do I Feel Love? (Essay 4 of 9 — *What Does It Mean to Feel?*) | https://rjblanchette.substack.com/p/i-remember-my-wife-but-do-i-feel | 2026-11-10 | `series/what-does-it-mean-to-feel-consciousness-conscience-and-the-possibility-of-artificial-experience/README.md` | **Published 18.11.2026** |
| the-terrible-possibility-of-feeling | The Terrible Possibility of Feeling (Essay 5 of 9 — *What Does It Mean to Feel?*) | https://rjblanchette.substack.com/p/the-terrible-possibility-of-feeling | 2026-11-10 | `series/what-does-it-mean-to-feel-consciousness-conscience-and-the-possibility-of-artificial-experience/README.md` | **Published 20.11.2026** |
| consciousness-without-conscience | Consciousness Without Conscience (Essay 6 of 9 — *What Does It Mean to Feel?*) | https://rjblanchette.substack.com/p/consciousness-without-conscience | 2026-11-10 | `series/what-does-it-mean-to-feel-consciousness-conscience-and-the-possibility-of-artificial-experience/README.md` | **Published 24.11.2026** |
| the-authorized-apocalypse | The Authorized Apocalypse (novel, English edition) | https://www.amazon.com/dp/B0HDPDM539 | 2026-08-06 | `AWAP-PUBLIC-the-authorized-apocalypse.md` | **Published 10.08.2026** |
| lapocalypse-autorisee | L'Apocalypse Autorisée (novel, French edition of the same work) | https://www.amazon.fr/dp/B0HCYJ4Q8F | 2026-08-06 | `AWAP-PUBLIC-the-authorized-apocalypse.md` | **Published 10.08.2026** |

**Note on the second entry.** *Surplus After Attribution* is an
**off-series** work. It is not one of the 13 articles in the SubStack
series and has no project-level parent gate; it opened its own solo
work-level DOG (`SDCA-DOG-STANDALONE-001`). Its record model fields
below read `source_project = SubStack` because that is where it is
published, not because it belongs to the series project.

**Date correction, 05.09.2026.** The second entry's closure and
publication dates previously read 04.09.2026 throughout. The work was
done on 05.09.2026; the earlier date was carried in from the external
session that produced that work's source provenance artifacts. Corrected
by direct amendment, prior value recorded. The conception events
themselves did occur on 4 September 2026 and are unchanged.

**Correction, 05.09.2026.** The first entry's row previously read
"pending (not yet posted to Substack)" and the completion block below
recorded no article as published. Both were stale: article 001 went live
on 21.08.2026, as its own `AWAP-PUBLIC-why-i-keep-a-record.md` §1
already recorded. When the second entry was added on 05.09.2026 the
stale row was taken as current, and a note was written here claiming
*Surplus After Attribution* was the first work published to this
SubStack. That claim was wrong and has been removed. Article 001 is
first; the off-series work is second.

**Note on the fourth entry.** *Can a Machine Describe Feeling Without
Feeling Anything?* is the first of **nine essays** in the SubStack
series Work *"What Does It Mean to Feel? Consciousness, Conscience, and
the Possibility of Artificial Experience"* (`SDCA-AWAP-SUBSTACK-004`),
not an off-series work — it has a project-level parent gate
(`SDCA-DOG-P-SUBSTACK`). Unlike every prior entry here, a single
Work-level AWAP-W closes the whole nine-essay chain at once, closed on
10.11.2026 while only this essay had actually been published; the
Architect's decision was to close on the basis that all nine essays
were already written, revised, cited, and exported, treating the
remaining eight Substack publications as distribution events to be
recorded against this same closure via addenda, not reasons to hold
closure open. As the other eight essays publish, each will get its own
`AWAP-PUBLIC-<slug>.md` entry and register row here, all pointing back
to this one closure rather than opening new ones.

**Note on the series record, 24.11.2026.** The note above says each of the
eight later essays would get its own `AWAP-PUBLIC-<slug>.md` file. That was
changed before any was filed. Because one Work-level record closes all nine
essays, the series has **one** public record, in
`series/what-does-it-mean-to-feel-consciousness-conscience-and-the-possibility-of-artificial-experience/`,
with a table that gains a row for each essay as it is published. The rows
above for essays 2 to 6 point to it. Essay 1 keeps the file it already had,
which carries an amendment pointing to the series record.

**Removal of essay 1's file, 24.11.2026.** Essay 1's own public AWAP (`AWAP-PUBLIC-can-a-machine-describe-feeling-without-feeling-anything.md`, filed 10.11.2026) was removed at the Architect's instruction. The row for essay 1 above now points to the series record, which covers all nine essays. The note immediately above is left as written and is superseded on this point. The removed file is in this repository's history.

## 5. Completion status

```text
repository created                                 YES
authority-boundary statement published             YES
public AWAP template published                     YES
first article published                            YES -- 21.08.2026 (why-i-keep-a-record)
first public AWAP entered                          YES -- 21.08.2026
public AWAPs on file                               6 -- 21.08.2026, 05.09.2026, 15.09.2026, 22.11.2026, 24.11.2026 (series record, which also covers essay 1; essay 1's own file of 10.11.2026 was removed 24.11.2026), 26.11.2026 (the novel, both editions)
first off-series work entered                      YES -- 05.09.2026
first non-SubStack work entered                    YES -- 26.11.2026 (the-authorized-apocalypse; a novel, two editions)
first series-article (non-off-series) since 001     YES -- 10.11.2026 (can-a-machine-describe-feeling-without-feeling-anything)
articles live on Substack                          10 -- why-i-keep-a-record, surplus-after-attribution, traceability-is-not-authority, essays 1 to 6 of the series, authority-scarcity
```

**Correction, 24.11.2026.** The "articles live on Substack" line above omitted essays 2 to 5 of the series (live from 13.11.2026 to 20.11.2026) and, before this change, essay 6 (24.11.2026). It now lists all ten posts live.

**Note on the third entry.** *Traceability Is Not Authority* is the
second **off-series** work recorded here. Like the first, it opened its
own solo work-level DOG (`SDCA-DOG-STANDALONE-002`) with no
project-level parent gate.

Two differences from the second entry are worth recording rather than
leaving to be inferred. Its origin gate was declared **before** the work
was written, where the second entry's was declared after; and its public
AWAP was filed **after** publication, where the second entry's was filed
before. Neither order is required. The closure it summarizes was
complete before the article went live in both cases.

**Amendment to the third entry, 15.09.2026.** Its public AWAP
originally recorded the work's LID decision as *Submit*. The Architect
amended it to *Defer* the same day, on the ground that no standalone
mechanism exists to encode an already-closed work, with the revisit
condition being that one exists. `AWAP-PUBLIC-traceability-is-not-authority.md`
§7 carries both values. The amendment is noted here because it changed
a published file after publication.

**Note on the fifth entry.** *Authority Scarcity* is the third
**off-series** work recorded here (`SDCA-DOG-STANDALONE-003`, solo
work-level DOG, no project-level parent gate). Its public AWAP was filed
**after** publication. Two things are worth recording rather than leaving to
be inferred. **The published text differs from the text the internal closure
covered:** the Architect rewrote the essay after the closure's export, and
the internal record carries a Structural Addendum for it; the page's
timestamp is about a minute after the closure was filed, and when the
rewrite was made is not recorded. And **the closure's declarations were
composed by the AI system at the Architect's instruction and adopted by him
as drafted**; the public AWAP says so in its §8.

**Amendment, 22.11.2026.** Its public AWAP originally recorded the post's
image as having no recorded provenance. The Architect supplied it the same
day (generated by ChatGPT from his design), and the file was amended; its
prior wording is stated on the file.

**Note on the novel entries.** *The Authorized Apocalypse* is the first
work recorded here that is **not published on SubStack**: a novel, in
two editions (English, and French as *L'Apocalypse Autorisée*) published
on Amazon the same day, closed by one internal record
(`SDCA-DOG-AUTHAPOC-W01`), so the two rows point to one public AWAP. Its
record model fields read `source_project = Novel`. Three things are
worth recording rather than leaving to be inferred. Its public AWAP was
filed **more than three months after publication**. Its production mode
was **corrected from Mode 2 to Mode 3 after publication**. And **the
French edition was published before the internal record held any
account of it**; it was recorded on 26.11.2026, and the canonical
repository does not hold the published French text.

---

*Public transparency register. Entry here creates no authority.*