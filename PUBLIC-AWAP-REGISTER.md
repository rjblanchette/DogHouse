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
| can-a-machine-describe-feeling-without-feeling-anything | Can a Machine Describe Feeling Without Feeling Anything? (Essay 1 of 9 — *What Does It Mean to Feel?*) | https://rjblanchette.substack.com/p/can-a-machine-describe-feeling-without | 2026-11-10 | `AWAP-PUBLIC-can-a-machine-describe-feeling-without-feeling-anything.md` | **Published 10.11.2026** |
| authority-scarcity | Authority Scarcity: The Constitutional Challenge of the AI Age | https://rjblanchette.substack.com/p/authority-scarcity | 2026-11-22 | `AWAP-PUBLIC-authority-scarcity.md` | **Published 22.11.2026** |

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

## 5. Completion status

```text
repository created                                 YES
authority-boundary statement published             YES
public AWAP template published                     YES
first article published                            YES -- 21.08.2026 (why-i-keep-a-record)
first public AWAP entered                          YES -- 21.08.2026
public AWAPs on file                               5 -- 21.08.2026, 05.09.2026, 15.09.2026, 10.11.2026, 22.11.2026
first off-series work entered                      YES -- 05.09.2026
first series-article (non-off-series) since 001     YES -- 10.11.2026 (can-a-machine-describe-feeling-without-feeling-anything)
articles live on Substack                          5 -- why-i-keep-a-record, surplus-after-attribution, traceability-is-not-authority, can-a-machine-describe-feeling-without-feeling-anything, authority-scarcity
```

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

---

*Public transparency register. Entry here creates no authority.*