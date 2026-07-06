---
paper_id: GITHUB-ALMANACIC-ZINE-HOST-v0.002
title: "GitHub as an Almanacic Zine Host"
subtitle: "Repositories as Living Public Scholarship"
author: "Lumixdeee with QA-DRC"
date: "2026-07-06"
version: "v0.002"
status: "method paper draft for review"
---

# GitHub as an Almanacic Zine Host

## Repositories as Living Public Scholarship

**Version:** v0.002  
**Status:** method paper draft for review  
**Scope:** publication-form method for living public scholarship. Not a claim that every paper belongs on GitHub. Not a preservation guarantee. Platform facts should be checked against current GitHub documentation before release.

## Abstract

A GitHub repository is usually treated as code storage, software collaboration space, or backstage infrastructure for a finished publication. This paper argues for another use: the repository as an almanacic zine host.

In this mode, the repository is not only where a public object is stored. It is part of the object. The README acts as front door and route card. Folders act as rooms. Issues act as reader letters, errata, source challenges, and open questions. Pull requests act as staged repair. Branches act as alternate editions. Tags and releases act as numbered drops. Permanent links pin a cited state. A reader-facing site gives a front surface without cutting the source trail away.

The paper separates metaphor from method. Calling a commit "marginalia" is not enough. The method test is whether repository mechanics change what a reader may cite, what a contributor may repair, what an owner may govern, and what a future reader may re-open.

The keeper:

```text
A repo-zine passes when the workshop changes the publication.
```

## 0. One-minute operator

Before calling a repository a zine, make it produce a receipt.

```text
REPO_ZINE_RECEIPT={
  object:
  audience:
  current_edition:
  start_path:
  source_shelf:
  repair_route:
  citation_state:
  issue_drop:
  maintainer_route:
  export_path:
  what_the_repo_lets_readers_do:
  what_a_flat_artifact_would_hide:
  failure_class:
}
```

Allowed claim:

```text
This repository hosts a living public object because its mechanics
govern reading, repair, citation, release, and re-opening.
```

Blocked claim:

```text
This repository is a zine because the folders have cute names.
```

## 1. Core claim

The working claim is small.

```text
REPO != ONLY_CODE_STORAGE
REPO_ZINE != FILE_DUMP
ZINE_LABEL != METHOD
WORK_SURFACE_CAN_BE_PART_OF_PUBLICATION
```

A repo-zine is a public knowledge object whose files, route map, versions, repairs, questions, and reader participation live in one repository.

The claim is not that GitHub was designed for zines. The claim is that some public scholarship needs a front edition and a work surface at once. Flattening those objects into one PDF, one blog post, or one frozen page can lose repair state, source state, reader letters, and version route.

Good candidate objects include:

```text
living bibliographies
public methods
teaching packs
field notebooks
community archive packets
conlang grammars
errata ledgers
data dictionaries
local history almanacs
multi-version public essays
paper families with source maps
```

These objects are not only text. They carry recurrence, source state, dispute state, repair tickets, reader routes, and future openings.

## 2. H0 and test

H0:

```text
GitHub is only code storage, software collaboration,
issue tracking, and static site hosting.
The zine / almanac reading is decorative.
```

Working claim:

```text
H0 loses force when ordinary repository mechanics do publication work
that a flat artifact does not do as cheaply.
```

Test:

```text
Does the mechanic change citation, repair, governance, reader route,
release state, or source custody?
```

If the answer is no, the zine language is decoration.  
If the answer is yes, the repository is doing publication work.

## 3. Source base and receipt

The platform side of this paper is grounded in GitHub documentation. The draft uses GitHub documentation on README files, Issues, forks, wikis, releases, permanent links, and Pages. The zine and archive side uses scholarship on zines as community archive practice and visualization medium. The citation side aligns with software and data citation work that treats versioned digital objects as citeable scholarly objects.

Source use should remain receipt-shaped:

```text
SOURCE_CARD={
  source:
  platform_fact_or_scholarship_claim:
  job_in_argument:
  claim_supported:
  claim_not_supported:
}
```

A GitHub documentation page can support a platform fact. It does not prove the zine reading by itself. A zine-scholarship source can support the public-form lineage. It does not prove GitHub is the right host. The method emerges from the feature-to-job map.

## 4. Repo-zine grammar

A repo-zine needs grammar because a platform feature can be decoration or method.

| Repo part | Zine / almanac job | Method test |
|---|---|---|
| `README.md` | front door, masthead, route card | New reader learns object, status, start path, owner, citation route. |
| `START_HERE.md` | first path | Reader does not have to infer entry from tree shape. |
| `/issues/` | numbered editions | Items have dates, version IDs, audience, and release notes. |
| GitHub Issues | letters, errata, source challenges | Reader input changes route state or repair state. |
| Pull requests | staged repair | Proposed edits can be inspected before entering the main edition. |
| Branches | alternate editions | Experiments remain available without replacing front edition. |
| Tags | named moments | A state can be named without guessing. |
| Releases | public drops | A package is frozen with notes, assets, and known open questions. |
| Permanent links | citation pins | A cited claim points to the same file state later. |
| `/evidence/` | source shelf | Evidence is separated from texture, jokes, and wall material. |
| `/errata/` | repair ledger | Corrections do not vanish after merge. |
| `/docs/` or Pages | reader surface | Nontechnical reading surface stays near source state. |

The grammar rejects the PDF-only model without rejecting PDFs. A PDF can be a reader edition. The repo holds the work surface around it.

## 5. Metaphor versus method

### Metaphor only

```text
README = cover
but it does not name status, route, version, owner, or citation form.

Issues = letters
but reader notes never enter repair state.

Releases = zine issues
but the release has no edition note, open questions, or source state.

Branches = alternate timelines
but no branch has a job, merge rule, or archive status.
```

### Method

```text
README = cover
because it names object, audience, start path, current edition,
maintenance route, citation form, and error route.

Issue = letter
because it can be labeled as erratum, source challenge,
reader note, or open question.

Release = issue
because it freezes a numbered edition with assets, date,
notes, source state, and open questions.

Branch = alternate edition
because it holds an experiment with a route back to main,
archive, merge, or refusal.
```

The method is behavioral. The test is what the repository lets people do.

## 6. Almanac logic

An almanac is recurring public knowledge with date, season, practical route, and return.

A repo-zine borrows that recurrence.

```text
monthly issue
seasonal source map
annual repair ledger
dated route note
versioned glossary
open questions carried forward
reader letters grouped by edition
```

This gives living scholarship rhythm. The object may change, but the change arrives through named drops rather than silent replacement.

A repository makes this cheap:

```text
tags name the moment
releases package the issue
commits show the path
issues carry unresolved items
branches hold experiments
Pages presents a reader surface
```

The almanac form matters because many public knowledge objects return. They are not finished once.

## 7. Worked example: river-town almanac

A public local-knowledge repo might look like this:

```text
river-town-almanac/
  README.md
  START_HERE.md
  STATUS.md
  CITATION.cff
  CHANGELOG.md
  /issues/
    2026-07-summer-water.md
    2026-10-autumn-wind.md
  /rooms/
    river.md
    garden.md
    birds.md
    recipes.md
    folklore.md
  /evidence/
    source_map.md
    water_log.md
    oral_history_register.md
  /errata/
    open.md
    repaired.md
  /.github/
    ISSUE_TEMPLATE/
      erratum.yml
      field-note.yml
      reader-letter.yml
      source-challenge.yml
  /docs/
    index.md
```

This repository is not a storage bin.

```text
README.md:
  names object, audience, current edition, owner route, citation form

START_HERE.md:
  gives routes for resident, teacher, contributor, reviewer

/issues/2026-07-summer-water.md:
  acts as the July edition

/evidence/source_map.md:
  states what each claim depends on

/errata/open.md:
  keeps unsettled items visible

release v2026.07:
  freezes the July issue

commit permalink:
  pins the water_log.md state cited by a paragraph

branch autumn-redesign:
  holds an alternate edition while main remains stable
```

That is method, not metaphor, because platform mechanics decide reading, repair, and citation.

## 8. Custody rules

### Rule 1: front door first

The README must answer:

```text
What is this?
Who is it for?
What is current?
Where should a new reader start?
How should this be cited?
How should errors be reported?
Who maintains it?
What is outside this repo?
```

### Rule 2: folders need jobs

Folders should not be named only for texture. Each folder needs a job and a route note.

```text
/evidence/ = source shelf
/errata/ = repair ledger
/issues/ = public editions
/rooms/ = topic spaces
/docs/ = reader-facing site source
/archive/ = old editions kept for custody
```

### Rule 3: releases are issues

A release should say:

```text
edition
date
files included
what changed
what remains open
assets
citation route
known export locations
```

### Rule 4: questions stay visible

Open questions should not vanish because they are unfinished. They should be marked with status, owner route, and next valid move.

### Rule 5: source and decoration separate

A sticker, image, joke, mascot, or room label may help readers. It may not masquerade as evidence. Evidence lives in the source shelf.

### Rule 6: cite state, not only location

Branch links can move with new commits. Claims depending on exact text should cite a tag, release, DOI deposit, or commit permanent link.

### Rule 7: forks are editions

A fork may be a translation, local edition, classroom edition, disputed edition, or repair experiment. It is not only a technical copy.

### Rule 8: platform is not preservation

A repo-zine needs export. Markdown, release packages, PDFs, citation files, and outside deposits keep the object from being trapped inside one platform.

## 9. Failure taxonomy

| Failure | Shape | Repair |
|---|---|---|
| Maze repo | Many files, no first path. | Add README, START_HERE, folder route notes. |
| Dead workshop | Claims living status, no current route. | Add STATUS, release cadence, active/archive label. |
| Source cosplay | Citations appear without claim-to-source map. | Add source map with claim, source, state, status. |
| Sticker takeover | Mascots, rooms, jokes become the object. | Separate wall material from source and route material. |
| Platform captivity | Object only works inside one interface. | Keep exportable Markdown, PDF, release package, citation file. |
| Infinite draft | Repo never drops an edition. | Use dated release intervals. |
| Silent replacement | Front text changes without reader-facing note. | Use changelog and release notes naming object-level changes. |
| Issue swamp | Issues pile up without labels or owner route. | Add issue templates, labels, status, triage rhythm. |
| Fork fog | Forks exist but no edition relation is named. | Name fork role: translation, local edition, experiment, dispute. |
| Citation drift | Reader cannot reach cited state later. | Use tag, release, DOI deposit, or commit permalink. |

## 10. Academic use

Repo-zines fit scholarly cases where the finished object and route both matter.

### Public methods

A methods paper often hides failed branches, source arguments, and repair choices. A repo-zine can publish the method paper, protocol, source map, errata ledger, and issue history as one object with several surfaces.

### Living bibliographies

A bibliography changes. A repo-zine can release dated bibliography issues, accept source challenges through issue templates, and keep rejected additions visible with reasons.

### Teaching packs

A teacher may need a stable handout and active repair surface. Releases provide class editions. Issues carry student questions and errata. Pages gives a reader surface.

### Community archive packets

Community archive work may need shared stewardship, local language, photos, oral histories, annotations, and contestation. A repository can make selected process visible without dumping the whole archive onto every reader.

### Nonlinear essays

Some arguments have rooms, not chapters. A repo-zine lets a reader choose the front essay, source shelf, glossary, errata room, or discussion wall.

## 11. Relation to scholarly infrastructure

The repo-zine does not replace journals, archives, DOI registries, institutional repositories, or data repositories. It adds a work surface before, beside, and after them.

A journal article may be the sanctioned edition. A repository may hold:

```text
source maps
version notes
review replies
supplements
teaching editions
errata
reader letters
public protocols
```

The repo-zine is strongest when paired with external archival deposits and citation records.

## 12. Minimal template

A small repo-zine needs route, not ornament.

```text
repo-zine/
  README.md
  START_HERE.md
  STATUS.md
  CITATION.cff
  CHANGELOG.md
  /issues/
    issue-001.md
  /evidence/
    source_map.md
  /errata/
    open.md
    repaired.md
  /docs/
    index.md
```

Minimal README sections:

```text
Object
Audience
Current edition
Start path
Citation
How to report an error
Folder map
Maintenance status
License
```

Minimal issue labels:

```text
erratum
source challenge
reader letter
field note
route problem
edition proposal
```

Minimal release note:

```text
Edition
Date
Files included
What changed
Open questions
Citation
Known export locations
```

## 13. Scoring sheet

A repo-zine can be scored before release.

| Field | 0 | 1 | 2 |
|---|---|---|---|
| Front door | absent | names object | names object, audience, current edition, start path |
| Source shelf | absent | sources listed | claims mapped to source state |
| Repair route | absent | contact route | issue templates, labels, errata ledger |
| Edition state | loose files | dated files | releases/tags with notes and assets |
| Citation state | moving links | general citation | tag, release, commit link, DOI, or deposit route |
| Reader surface | only tree | README only | Pages or docs plus source route |
| Governance | unknown | maintainer named | owner route, change rule, archive rule |
| Export | platform-only | manual download | release package, PDF/MD, citation file, outside deposit path |

Interpretation:

```text
0-4:
  file pile

5-9:
  public repo with some route

10-13:
  repo-zine candidate

14-16:
  working repo-zine
```

The score is not prestige. It is custody pressure.

## 14. Discussion

The repo-zine model matters because it treats route as publication material. Many scholarly artifacts already have route, but route is hidden in drafts, email, notebooks, commit history, chat transcripts, reviewer exchanges, and file names.

A repo-zine does not expose everything. It exposes the parts that help readers understand state, repair, and citation.

This is governance as much as format. The author states what may be changed, what must be frozen, what counts as repair, how reader input enters, and how a future reader reaches the cited state.

The main discipline is smallness. A repo-zine should not eat every note. It should keep the public object, its route, and its repair ledger near each other. Cold archive material may remain outside the active surface with an index.

## 15. Limits and next build

Limits:

```text
GitHub is not a preservation guarantee.
A public repo does not equal public scholarship.
Issue traffic does not equal reader participation.
Cute labels do not create method.
Commit history does not replace source maps.
Living status can become infinite draft.
```

Next build:

```text
verify current GitHub documentation against platform facts;
add a one-page repo-zine setup template;
add a worked README;
add issue templates;
add release-note template;
make a small demo repository structure;
test with a nontechnical reader;
test citation-state recovery from an old paragraph.
```

## 16. Conclusion

GitHub is underused as a host for living public scholarship because it is often read too narrowly. Its ordinary machinery already carries many jobs of zines and almanacs: self-publication, recurrence, reader letters, repair, alternate editions, source pinning, and issue-based release.

The repo-zine is not a brand. It is a method for objects that need a front edition and a work surface. The workshop can be part of the publication when the route is named, the source shelf pays rent, and the cited state can be reached again.

Keeper:

```text
The README opens the door.
The release freezes the issue.
The source shelf pays rent.
The errata room keeps repair visible.
The cited state must be reachable later.
```

## Local source packet

This v0.002 is revised from the uploaded v0.001 draft and its local anchors:

```text
extra_extra_expanded/NAK_github_as_non_linear_almanacic_zine_host_v0_001.md
extra_extra_expanded/github_zine_b_pass_v0_002_bundle__unzipped/github_zine_almanac_B_custody_pass_v0_002.md
extra_extra_expanded/github_zine_b_pass_v0_002_bundle__unzipped/github_zine_almanac_B_source_rent_v0_002.csv
extra_extra_paper_strike_update.md
```

## References

[1] GitHub Docs. "About the repository README file." https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes

[2] GitHub Docs. "About issues." https://docs.github.com/articles/about-issues

[3] GitHub Docs. "About forks." https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/about-forks

[4] GitHub Docs. "About wikis." https://docs.github.com/en/communities/documenting-your-project-with-wikis/about-wikis

[5] GitHub Docs. "Adding or editing wiki pages." https://docs.github.com/en/communities/documenting-your-project-with-wikis/adding-or-editing-wiki-pages

[6] GitHub Docs. "Managing releases in a repository." https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository

[7] GitHub Docs. "Getting permanent links to files." https://docs.github.com/en/repositories/working-with-files/using-files/getting-permanent-links-to-files

[8] GitHub Docs. "What is GitHub Pages?" https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages

[9] Baker, S., and Cantillon, Z. "Zines as community archive." *Archival Science* 22, 539-561, 2022. https://doi.org/10.1007/s10502-022-09388-1

[10] McNutt, A. "On the Potential of Zines as a Medium for Visualization." arXiv:2108.02177, 2021. https://arxiv.org/abs/2108.02177

[11] Smith, A. M., Katz, D. S., Niemeyer, K. E., and FORCE11 Software Citation Working Group. "Software citation principles." *PeerJ Computer Science* 2:e86, 2016. https://doi.org/10.7717/peerj-cs.86

[12] Wilkinson, M. D., Dumontier, M., Aalbersberg, I. J. J., et al. "The FAIR Guiding Principles for scientific data management and stewardship." *Scientific Data* 3, 160018, 2016. https://doi.org/10.1038/sdata.2016.18
