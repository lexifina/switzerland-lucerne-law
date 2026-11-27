<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Deutsch](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Lucerne only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-27 06:33 UTC, Lucerne: systematic collection (srl.lu.ch): 300 addresses read; 0 added, 0 changed, 0 removed; no change; 39 not published, 0 of them with no reason.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [Lucerne: systematic collection (srl.lu.ch)](https://srl.lu.ch/) | `<act>/` | daily | 2026-11-27 06:33 UTC | no change | watched |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-27 06:28](checks/2026-11.md#ch-lexwork-lucerne-20261127t062833z) | lexwork-lucerne | 300 | 0 | 0 | 0 | 39 (0) | no change | — |
| [2026-11-26 06:31](checks/2026-11.md#ch-lexwork-lucerne-20261126t063135z) | lexwork-lucerne | 98 | 0 | 0 | 0 | 44 (0) | no change | — |
| [2026-11-25 07:03](checks/2026-11.md#ch-lexwork-lucerne-20261125t070306z) | lexwork-lucerne | 447 | 127 | 0 | 0 | 44 (0) | changes found | [297](https://github.com/lexifina/switzerland-lucerne-law/compare/2438dbf24230...922d7128acdc) |
| [2026-11-24 14:49](checks/2026-11.md#ch-lexwork-lucerne-20261124t144910z) | lexwork-lucerne | 500 | 161 | 3 | 0 | 164 (0) | the check failed | — |
| [2026-11-24 12:09](checks/2026-11.md#ch-lexwork-lucerne-20261124t120903z) | lexwork-lucerne | 253 | 161 | 2 | 0 | 165 (0) | the check failed | — |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
