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
| why-i-keep-a-record | Why I Keep a Record When I Work With AI | pending (not yet posted to Substack) | 2026-08-21 | `AWAP-PUBLIC-why-i-keep-a-record.md` | Closure filed, publication pending |
| surplus-after-attribution | Surplus After Attribution | https://rjblanchette.substack.com/p/surplus-after-attribution | 2026-09-04 | `AWAP-PUBLIC-surplus-after-attribution.md` | **Published 04.09.2026** |

**Note on the second entry.** *Surplus After Attribution* is an
**off-series** work. It is not one of the 13 articles in the SubStack
series and has no project-level parent gate; it opened its own solo
work-level DOG (`SDCA-DOG-STANDALONE-001`). Its record model fields
below read `source_project = SubStack` because that is where it is
published, not because it belongs to the series project.

## 5. Completion status

```text
repository created                                 YES
authority-boundary statement published             YES
public AWAP template published                     YES
first article published                            YES -- 04.09.2026
first public AWAP entered                          YES -- 21.08.2026
public AWAPs on file                               2 -- 21.08.2026, 04.09.2026
first off-series work entered                      YES -- 04.09.2026
articles live on Substack                          1 -- surplus-after-attribution
```

**Note.** The first work published to Substack is the off-series
*Surplus After Attribution*, not the series' own article 001. Article
001's closure and public AWAP were filed first, on 21.08.2026, but its
Substack post is not yet live.

---

*Public transparency register. Entry here creates no authority.*
