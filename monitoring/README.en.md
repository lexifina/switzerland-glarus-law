<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Deutsch](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Glarus only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-27 06:18 UTC, Glarus: systematic collection (gesetze.gl.ch): 188 addresses read; 0 added, 1 changed, 0 removed; changes found; 7 not published, 0 of them with no reason.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [Glarus: systematic collection (gesetze.gl.ch)](https://gesetze.gl.ch/) | `<act>/` | daily | 2026-11-27 06:18 UTC | changes found | watched |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-27 06:14](checks/2026-11.md#ch-lexwork-glarus-20261127t061448z) | lexwork-glarus | 188 | 0 | 1 | 0 | 7 (0) | changes found | — |
| [2026-11-26 06:21](checks/2026-11.md#ch-lexwork-glarus-20261126t062118z) | lexwork-glarus | 79 | 0 | 0 | 0 | 5 (0) | no change | — |
| [2026-11-25 06:45](checks/2026-11.md#ch-lexwork-glarus-20261125t064513z) | lexwork-glarus | 255 | 129 | 0 | 0 | 5 (0) | changes found | [211](https://github.com/lexifina/switzerland-glarus-law/compare/0c2e59621dab...82f3b815ba98) |
| [2026-11-24 14:44](checks/2026-11.md#ch-lexwork-glarus-20261124t144444z) | lexwork-glarus | 178 | 129 | 0 | 0 | 132 (0) | the check failed | — |
| [2026-11-24 12:06](checks/2026-11.md#ch-lexwork-glarus-20261124t120603z) | lexwork-glarus | 279 | 132 | 1 | 0 | 139 (0) | the check failed | — |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
