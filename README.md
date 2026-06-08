# Free Job Candidate Screener Using Claude Projects

A free, open-source AI-powered candidate screening tool built on [Claude Projects](https://claude.ai). No code required. Works two ways — for HR teams screening candidates, and for candidates reviewing their own resume against a job description.

---

## What it does

### For HR / Recruiters
Paste a job description → upload a resume → get a full screening report in seconds.

- Every must-have and nice-to-have skill rated out of 10 with evidence from the resume
- Responsibility match analysis per JD bullet point
- Weighted overall match score
- Interactive spider chart — candidate scores vs JD baseline
- Clear hiring recommendation: ✅ Recommend / ⚠️ Reservations / ❌ Do Not Recommend
- Screen multiple candidates against the same JD in one session with a side-by-side comparison table

### For Candidates
Upload your resume → paste a job description → get an honest gap analysis.

- See exactly where your resume is strong and where it falls short for the specific role
- Understand which gaps are critical vs which are nice-to-have
- Get a concrete resume improvement action plan with specific wording suggestions
- Spider chart showing your profile vs what the role actually needs

---

## How to set up (5 minutes, free)

### What you need
- A [Claude.ai](https://claude.ai) account (free tier works)
- The two files from this repo: `project-instructions.md` and `scoring-rubric.md`

### Setup steps

1. Go to [claude.ai](https://claude.ai) and sign in
2. Click **Projects** in the left sidebar → **New Project**
3. Name it: `Job Candidate Screener` (or anything you like)
4. Click **Project Instructions** → paste the full contents of `instructions/project-instructions.md`
5. Click **Project Files** → upload `instructions/scoring-rubric.md`
6. Done — start a new chat inside the project to begin screening

> **No Claude Pro required for basic use.** Large PDF resumes or very long JDs may hit free tier context limits. If that happens, paste the resume as plain text instead of uploading.

---

## How to use

### HR / Recruiter flow

```
1. Start a new chat inside the project
2. Paste the job description
3. Claude confirms it and lists the extracted requirements
4. Upload the candidate's resume (PDF, DOCX, or paste as text)
5. Claude generates the full screening report + spider chart
```

To screen a second candidate against the same JD: just upload another resume in the same chat. Claude will generate a new report and add a side-by-side comparison table.

### Candidate flow

```
1. Start a new chat inside the project
2. Upload your resume (PDF, DOCX, or paste as text)
3. Claude confirms it and asks for the job description
4. Paste the job description
5. Claude generates your gap analysis + resume improvement action plan + spider chart
```

---

## What the report includes

| Section | HR Report | Candidate Report |
|---|---|---|
| 1 | Candidate snapshot | Your profile summary |
| 2 | JD requirements rating table (scored /10 with evidence) | Where you stand on each requirement |
| 3 | Additional skills from resume | What you bring beyond the JD |
| 4 | Responsibility match analysis | Where your experience aligns or falls short |
| 5 | Overall weighted score summary | Your overall match score |
| 6 | Interactive spider chart (downloadable PNG) | Interactive spider chart (downloadable PNG) |
| 7 | Hiring recommendation | Resume improvement action plan |

---

## Scoring methodology

All scores are **1–10**, evidence-based, applied consistently across both modes:

| Score | Meaning |
|---|---|
| 9–10 | Explicit senior-level or multi-year demonstrated expertise |
| 7–8 | Clear direct experience with context |
| 5–6 | Mentioned without strong context or inferred from adjacent skills |
| 3–4 | Brief or passing mention only |
| 1–2 | Completely absent or very loosely inferred |

**Overall score weighting:**
- Must-Have Skills: 40%
- Responsibility Match: 25%
- Nice-to-Have Skills: 15%
- Experience Level Fit: 12%
- Communication / Presentation: 8%

Full rubric: see `instructions/scoring-rubric.md`

---

## Files in this repo

```
├── README.md                          ← You are here
├── instructions/
│   ├── project-instructions.md        ← Paste this into Claude Project Instructions
│   └── scoring-rubric.md              ← Upload this as a Claude Project File
└── docs/
    └── example-report.md              ← Example output for a sample role
```

---

## Limitations

- Claude has no memory between separate project conversations. Each new chat starts fresh.
- Very long resumes (10+ pages) or JDs with 30+ requirements may need to be pasted as text rather than uploaded on the free tier.
- Scores reflect evidence in the resume only. Claude does not search the internet or verify claims.
- The spider chart is generated as an HTML artifact — use the Download PNG button to save it.
- This tool assists human judgment. It does not make hiring decisions.

---

## Contributing

Pull requests welcome. If you improve the scoring rubric, add support for a new resume format, or build a wrapper UI — open a PR with a clear description of what changed and why.

Please do not submit PRs that introduce company-specific branding, paid API dependencies, or bias toward any demographic group.

---

## License

MIT License — free to use, modify, and distribute. See `LICENSE`.

---

## Built with

- [Claude Projects](https://claude.ai) by Anthropic
- No code, no servers, no database
- Inspired by the need for accessible, unbiased screening tools for small teams and individual job seekers