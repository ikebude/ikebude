# TEST PLAN — `ikebude` profile README (docs workstream)

The tester runs this without relying on the builder's report. Branch `ccr-7d21c86c-pnbh8t`. Link checker:
`/tmp/claude-0/-home-user/e6ff3af4-b759-5a42-ae4a-d7f12c188d23/scratchpad/docs_links.py` (prints `BROKEN`/`OUTSIDE` lines; it skips code fences and `templates/`).

## A. Commands and expected results
| # | Command (run from /home/user/ikebude) | Expected |
|---|---|---|
| A1 | `git diff --stat origin/main..HEAD` | Only `README.md` and `tasks/*` changed. `assets/` untouched. |
| A2 | `python3 <scratchpad>/docs_links.py .` | no output |
| A3 | `grep -n -i "FX-Trading-Journal\|AI-Trading-Intelligence" README.md` | nothing |
| A4 | `grep -n -i "open-source\|banking\|3+ years\|In View\|live production\|live links" README.md` | nothing |
| A5 | `grep -c "deployment pending verification" README.md` | 3, unless a commit body holds curl proof of HTTP 200 for a site |
| A6 | visibility loop from BUILD_SPEC §5 | every linked ikebude repo is `public` |
| A7 | `git log --format='%an <%ae>' origin/main..HEAD \| sort -u` | only `ikebude <precious.ikebude@outlook.com>` |
| A8 | `git log --format=%B origin/main..HEAD \| grep -ci "opus\|claude"` | only matches from the two trailer lines (2 per commit) |

## B. Adversarial checks
1. **Anonymous 404 test:** for every `https://github.com/...` URL in the README, run `gh api repos/<owner>/<repo>` and, for tree/blob links, `gh api repos/ikebude/ai-ml-data-engineering/contents/<path>?ref=main`. Note: the case-study path `products/lolos-ledger` must exist on **main** of ai-ml-data-engineering (it does today).
2. **Markdown table integrity:** every table row in the "Featured" and "Industry" tables has the same number of `|` separators as its header (`awk -F'|' '/^\|/{print NR": "NF}' README.md`).
3. **Ownership not regressed:** row "Moniguard v2" still links `ikebude/MLOps-Fraud-Detection` (personal). The FraudGuard row is still under the 3Consulting heading and has no ikebude repo link (OWNER_DECISIONS.md #1).
4. **No new unverifiable claims:** diff only. Any new number or adjective like "production", "live" or "certified" in the diff is a FAIL.
5. **Render review:** view the rendered README (`gh api -X POST /markdown -f text="$(cat README.md)" -f mode=gfm > /tmp/r.html`, or GitHub's branch view) at 390 px and 1280 px widths, in light and dark. Check that the `<br/>` notes render and that no raw HTML leaks.

## C. README claim → evidence
| README claim | Evidence |
|---|---|
| "2+ years" experience | `/home/user/CV/BI Analyst/Precious.Ikebude.CV.docx` ("over 2 years"); employment Nov 2022 – Jan 2024 + 3Consulting (current). Owner to confirm. |
| No banking employer | none of the CVs list a bank; must not appear |
| Azure AI Engineer "In progress — target 2026" | owner statement; must not say obtained |
| Company sites "deployment pending verification" | `3Consulting-Who-I-am-working-for/README.md` hosting section; sandbox curl blocked (403 proxy) |
| Lolo's Ledger source private | `gh api repos/ikebude/AI-Trading-Intelligence -q .visibility` → private |
| Product benchmark numbers (lines 36–40, 79, 82) | **owned by the lead / other workstreams.** The tester lists any mismatch against product `reports/*.json` as a note, not a FAIL of this workstream |

## Tester findings
(append here: file:line, severity, description)
