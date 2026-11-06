# Lucerne: law history in git

Part of [lexifina/global-law](https://github.com/lexifina/global-law), one git history for every country's law: this is the law of Lucerne, Switzerland, which global-law reads at `switzerland/lucerne/acts/`.

The law of the canton of Lucerne (Kanton Luzern, Switzerland) as a git history: one file per article, one commit per amending act on the day it took effect, and the amending act as the commit's author. `git blame` names the act behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `ch-lu/`. The federal law is in [lexifina/switzerland-law](https://github.com/lexifina/switzerland-law).

The text is in German, the canton's official language, exactly as the canton publishes it.

## What this repository holds

The included acts and their recorded versions are listed in [data/versions.json](data/versions.json). That index defines the scope of each release. The collection covers the cantonal constitution and the indexed cantonal statutes, regulations, decrees, decisions and intercantonal agreements.

Where dated source versions are available, the record follows those versions. A current-text baseline records one consolidated text, dated by the source's own current-version in-force statement, with no reconstructed earlier history. Such a baseline is labelled "oldest version available" and is credited to the publisher.

Each act directory contains its own README with its title, source and version dates. Some individual corporation conversion or dissolution approvals, collection-district merger approvals and one-off funding approvals are outside the breadth extension because they perform completed individual actions. The historical collection retains the individual enactments already recorded there.

## Source

The SRL Nr. (systematic collection) of the canton, published by the canton at <https://srl.lu.ch/>. For each act it gives every consolidated version it holds, with the day each version took effect, and a change table listing each amendment: its decision date, the day it took effect, the provision it touched and its entry in the chronological collection (G). Separate PDF annexes are included where recorded in the act index; annex gaps in the earlier historical collection remain disclosed below.

## Dates

- Each commit is dated at **noon, Europe/Zurich, on the day the version took effect**, as the collection gives it ("in Kraft seit / von"). The decision date of each amending act is the `Enacted:` trailer.
- An act's first commit is its oldest version in the collection. It is credited to the act as enacted only when the change table shows no amendment in force before it; otherwise it is the "oldest version available", naming the earlier amendments.
- Versions that take effect after the retrieval day are on the `zukunft` branch, never merged into `main`.
- `--before="YYYY-MM-DD"` alone uses your clock's time of day; use `T23:59:59Z` or `tools/on.py`.

## Files

`<act>/art-005.md` is Art. 5 (or § 5), `art-005a.md` Art. 5a; `ingress.md` holds the title, date and preamble; `gliederung.md` the section headings; `schluss.md` the closing formula and signatures. One paragraph or list item per line. Amendment markers (`*`), footnote numbers and the "Stand" date are left out.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the canton's own text of that version, and every article's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the amending act, named by its entry in the chronological collection (G), with an e-mail address that cannot exist (`<act key>@srl.lu.ch.invalid`). Where one version holds changes by several amending acts and the change table does not say which provision each one touched, the commit names them all. The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one the canton publishes as binding (its chronological collection, or its systematic collection where cantonal law makes that binding). The history starts with the oldest consolidated version the collection holds for each act, which for many acts is later than the act's enactment. Only the acts listed above are included.

## Current texts and completeness

Current-text baselines are source texts, not reconstructed histories. XHTML baselines are single-file acts in source order. PDF records retain source page layout, including footnotes, hyphenation and page headers. Textual annexes are included where listed in the act index; source competence matrices retain their cells and column headings as textual tables.

Illustrations referred to but absent from the official source PDFs for SRL 737 and 785 remain deferred. Separate annex gaps in the earlier historical collection also remain. This collection does not claim complete illustration or annex coverage.
