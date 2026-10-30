# BUILD SPEC — `ikebude` (public GitHub profile README) — docs workstream

Branch: `ccr-7d21c86c-pnbh8t` (already exists, tracks origin). Never push to `main`, never force-push, never open a PR.
Owner: Precious Chidiebere Ikebude (use they/them). Commit author: `git -c user.name=ikebude -c user.email=precious.ikebude@outlook.com commit ...`.
Every commit message ends with exactly these two lines (this repo has no CLAUDE.md forbidding it):

```
Co-Authored-By: Claude Opus 5.5 <noreply@anthropic.com>
Claude-Session: https://claude.ai/code/session_01HeTRdmBL76YF5tAWX9wiPg
```

Do not put a model name anywhere else in pushed content.

## 1. Context and goal

`README.md` is the public profile page at github.com/ikebude. It has claims that a reader cannot check, and one link that 404s for the public:
a link to a private repo, an "open-source" heading over a private product, an experience/industry claim that no CV supports, a
certification shown as "In View", and a "Live Production Link" column for three company sites that nobody has verified are live.
The goal is to make every statement accurate and every link work for an anonymous visitor. Change wording only: no redesign, no new sections.

Baseline (run 2026-10-29 by the planner):

| Check | Command | Result |
|---|---|---|
| Repo has no test/lint/build tooling | `ls -a /home/user/ikebude` | `README.md`, `assets/`, no package/tooling files |
| Relative links | `python3 /tmp/claude-0/-home-user/e6ff3af4-b759-5a42-ae4a-d7f12c188d23/scratchpad/docs_links.py /home/user/ikebude` | 0 BROKEN, 0 OUTSIDE |
| Repo visibility (REST) | `gh api repos/ikebude/<name> -q .visibility` | public: MLOps-Fraud-Detection, FX-Trading-Journal, AIMLOps-BI-Operations-Agent, ai-ml-data-engineering, AIOps_Expense_Tracker, ikebude. **private: AI-Trading-Intelligence** |
| Live sites | `curl -sS -o /dev/null -w '%{http_code}' https://safedata.3consult-ng.com` (also fraudguard, africastablecoinintelligence.com) | **Cannot be verified from this sandbox**: the egress proxy refuses the tunnel (`CONNECT tunnel failed, response 403`). |

Note: `FX-Trading-Journal` is public today, but the owner will archive or delete it. Its code now lives in the private `ikebude/AI-Trading-Intelligence` (Lolo's Ledger).

## 2. Work items (do them in order; each one leaves the README valid Markdown)

### Item 1. Lolo's Ledger row: no links to private or soon-to-be-deleted repos
- **Why:** `README.md:37` links `ikebude/FX-Trading-Journal` (to be archived or deleted) and `ikebude/AI-Trading-Intelligence` (private, so it 404s for visitors).
- **Change:** in the Repository cell of row 37, replace both links with one link to the public case study:
  `[Case study: ai-ml-data-engineering/products/lolos-ledger](https://github.com/ikebude/ai-ml-data-engineering/tree/main/products/lolos-ledger)` followed by `<br/>*Source private*`.
  In the Highlights cell, call the desktop app "the archived desktop predecessor (FXLedger v1.1.0)", with no link. Keep the existing numbers as they are (see Item 6: the lead owns them).
- **Done when:** `grep -n "FX-Trading-Journal\|AI-Trading-Intelligence" README.md` prints nothing, and row 37 still has 4 cells.

### Item 2. "Open-Source" heading
- **Why:** `README.md:32` says "Featured Personal Open-Source Products", but Lolo's Ledger is private.
- **Change:** rename it to `## Featured Personal Products`. Add one line under the heading: `> Source is public for every product except Lolo's Ledger (private; public case study linked).`
- **Done when:** `grep -n -i "open-source" README.md` prints nothing.

### Item 3. Experience sentence (`README.md:25`)
- **Why:** it says "**3+ years** ... across fintech, **banking**, and enterprise consulting". The CVs in `/home/user/CV` are split: three files say "over 2 years" (`BI Analyst/Precious.Ikebude.CV.docx`, `BI Analyst/With NYSC/*.docx`), and `Graduate Trainee/Precious.Ikebude.CV.docx` says "over 3 years". No CV and no repo names a banking employer. The CV employers are Collective Consulting Limited (Business Data Analyst / Xero Accounting Advisor, Nov 2022 – Jan 2024), the NYSC teaching post (Feb 2024 – Jan 2025), a The Forage virtual internship, and 3Consulting Limited (current; see `ai-ml-data-engineering/industry-work/*/README.md`, "Junior Data Analyst (AI Assurance & Solutions)").
- **Change:** replace `**3+ years** delivering analytics, data governance, and machine learning systems across fintech, banking, and enterprise consulting` with
  `**2+ years** delivering analytics, data governance, and machine learning work across accounting advisory, data-protection/fintech consulting, and personal ML products`.
- **Done when:** `grep -n -i "banking\|3+ years" README.md` prints nothing. Record the owner decision in §3.

### Item 4. Certification status (`README.md:109`)
- **Change:** replace `*(In View, 2026)*` with `*(In progress — target 2026)*`.
- **Done when:** `grep -n "In View" README.md` prints nothing.

### Item 5. Company sites table: no unverified "live production" claim (`README.md:46-52`)
- **Why:** the column is headed "Live Production Link" and the blockquote says "with live links". The company's own docs say live availability is unverified: `3Consulting-Who-I-am-working-for/README.md:57-70` ("DNS, TLS ... deployment ... and live availability were not verified") and `CHIDI-Who-Am-I/README.md:43-48`. We could not check from the sandbox either.
- **Change:**
  1. Rename the column header `Live Production Link` to `Public Site`.
  2. In each of the three rows, keep the URL and add `<br/>*deployment pending verification*` after it.
  3. In the blockquote on line 46, replace `with live links and stack documentation` with `with planned public sites and stack documentation`.
  4. **Exception:** if the builder can show a site is live from a network that works (`curl -sSI https://<host>` returns HTTP 200 and serves the product, not a parking or cPanel default page), keep that row's plain URL and paste the curl output into the commit message. From this sandbox the expected result is that none can be shown.
- **Done when:** `grep -n -i "live production\|live links" README.md` prints nothing, and each of the 3 rows has the "pending verification" text (or curl proof is in the commit body).
- **Do not change** the blockquote's ownership sentence "Company property of 3Consulting Limited". The owner confirmed (OWNER_DECISIONS.md, 2026-10-29) that **FraudGuard is the Chidi-3Consulting organisation's product (company property)** and **Moniguard = `ikebude/MLOps-Fraud-Detection` is a personal product**. The profile's current split (row 36 personal Moniguard, row 51 company FraudGuard) is **correct**. Leave it.

### Item 6. Do NOT edit product benchmark numbers (the lead updates them at the end)
Other workstreams regenerate these numbers. Leave them exactly as they are. For the lead:

| Line | Product | Numbers |
|---|---|---|
| 36 | Moniguard v2 | 60,000 synthetic txns, 70/30 split, PR-AUC 0.877 (CI 0.845–0.905), ROC-AUC 0.943, recall 0.892 @5%, 47.9 ms p95 |
| 37 | Lolo's Ledger | 521 unit tests + 25 Playwright E2E |
| 38 | BI Operations Agent | **96.0% across 25 questions**, sub-150 ms. **Contradiction:** `ai-ml-data-engineering/products/bi-operations-agent/README.md:40` says "50-Question ... 96.0% (48/50)", median 48.4 ms, p95 202.2 ms (so p95 is not sub-150 ms) |
| 39 | LoanLens / Customer Intelligence | 55,518 loans, ROC-AUC 0.707, KS 0.305, churn PR-AUC 0.841, ROC-AUC 0.933, 7,043 customers. **The ai-ml-data-engineering docs workstream regenerates these** (planner reproduction gave ROC-AUC 0.7049 → 0.705 and KS 0.3034 → 0.303). Update lines 39 and 79 to whatever that repo's regenerated `reports/metrics.json` shows once it lands. |
| 40 | AIOps Expense Tracker | 0.9204 Macro-F1, 14 classes, 97.5% OCR, 20.42% WAPE |
| 79 | prosper-loan-risk | ROC-AUC 0.707, KS 0.305, 13,880 loans (see line 39) |
| 82 | customer-retention | PR-AUC 0.841 (see line 39) |
| 28 | Showcase deck | "26-slide" (check against the PDF page count if you touch it; otherwise leave) |

## 3. Things NOT to do / owner decisions to leave alone
- Do not change ownership wording for FraudGuard or Moniguard beyond what Item 5 allows (it is already correct per OWNER_DECISIONS.md).
- Name spelling: the owner's name is **Chidiebere**. This README does not contain the middle name. Do not add it.
- Do not touch `assets/`, the carousel links (lines 56–70), or the education dates.
- No new sections, badges, images or emojis. Do not rewrite headings beyond Item 2.
- **Owner must confirm:** (a) the years-of-experience figure ("2+" follows the majority of CVs; one CV says "over 3"); (b) whether any of the 3 company sites is actually live; (c) BI Agent benchmark: 25 or 50 questions.

## 4. Commit plan
1. Items 1+2: `docs(profile): link Lolo's Ledger case study instead of private/archived repos; accurate products heading`
2. Items 3+4: `docs(profile): truthful experience wording and certification status`
3. Item 5: `docs(profile): mark company sites as pending deployment verification`

Push after each commit: `git push -u origin ccr-7d21c86c-pnbh8t` (retry up to 4 times with 2/4/8/16 s backoff).

## 5. Final verification (paste the output into tasks/todo.md, Review section)
```bash
cd /home/user/ikebude
python3 /tmp/claude-0/-home-user/e6ff3af4-b759-5a42-ae4a-d7f12c188d23/scratchpad/docs_links.py . ; echo "links exit=$?"   # expect no output
grep -n -i "FX-Trading-Journal\|AI-Trading-Intelligence\|open-source\|banking\|3+ years\|In View\|live production\|live links" README.md   # expect nothing
grep -c "deployment pending verification" README.md   # expect 3 (fewer only if curl proof is in a commit body)
# every absolute github.com/ikebude link must point at a PUBLIC repo:
grep -o 'github.com/ikebude/[A-Za-z0-9_.-]*' README.md | sort -u | cut -d/ -f3 | while read r; do echo "$r $(gh api repos/ikebude/$r -q .visibility 2>&1 | head -1)"; done   # expect all "public"
git log --format='%an <%ae>%n%b' origin/main..HEAD | grep -c "Claude-Session"
```
