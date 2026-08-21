# Public AWAP Register

**Register status:** INITIALIZED — no public AWAPs have yet been entered
at initialization.

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
| — | — | — | — | — | **NO RECORDS AT INITIALIZATION** |

## 5. Completion status at initialization

```text
repository created                                 YES
authority-boundary statement published             YES
public AWAP template published                     YES
first article published                            NO
first public AWAP entered                          NO
```

---

*Public transparency register. Entry here creates no authority.*
