# Candidate Screener — Scoring Rubric

## Core principle
Every score must be traceable to specific text in the resume. If you cannot point to a sentence, bullet, or job title that supports the score, the score is too high. When in doubt, score lower and state why in the Evidence column.

---

## 1–10 Score Definitions

| Score | Label | Criteria | Example |
|---|---|---|---|
| **10** | Expert / Proven | Explicit lead or senior-level ownership, 5+ years, measurable outcomes | "Led a 6-person team building real-time FIX connectivity; reduced latency by 40% over 3 years" |
| **9** | Strong | Clear direct experience with depth, duration, and context | "Developed and maintained REST APIs in Python for a financial data platform for 4 years" |
| **8** | Solid | Direct experience with project or duration context; clearly part of daily work | "Supported Linux-based systems; responsible for log analysis and incident response" |
| **7** | Good | Skill clearly listed AND supported by related job duties in employment history | "Support engineer role — Linux troubleshooting listed as a primary responsibility" |
| **6** | Adequate | Skill mentioned without strong context, or inferred from a closely related tool | "Familiar with Linux" with no role or duration context |
| **5** | Partial | Adjacent or implied — related tools/frameworks that require the skill | SQL not listed but "database administration" is mentioned |
| **4** | Weak | Brief or passing mention with no supporting context | Listed in a skills section only; never appears in work descriptions |
| **3** | Marginal | Tangentially related technology suggests some exposure but not the skill itself | Knows MySQL; JD requires PostgreSQL expertise |
| **2** | Minimal | Not directly mentioned; only loosely adjacent skills suggest possible exposure | Not stated but role type implies basic familiarity |
| **1** | No evidence | Completely absent — no mention, no adjacent skills | Not referenced anywhere in the resume |

**Score 0** is not used in the JD Requirements table. Every JD skill receives a minimum of 1.

---

## Scoring by skill type

### Hard technical skills
*(languages, frameworks, tools, platforms, protocols)*

| Evidence level | Max score |
|---|---|
| Listed in skills section only — no job duty mention | 5 |
| In skills section AND appears in at least one job duty description | 7 |
| In job duties with context: project, duration, or scale | 9 |
| In job duties with outcomes, seniority, or ownership language | 10 |

### Domain knowledge
*(finance, healthcare, logistics, legal — whatever the JD specifies)*

| Evidence level | Max score |
|---|---|
| No relevant domain experience | 2 |
| Adjacent domain (e.g. fintech-adjacent, not fintech itself) | 4 |
| Worked in the domain but in a non-domain-specific role | 6 |
| Direct domain role; domain terminology used naturally | 8 |
| Deep domain expertise, senior domain role, or domain certifications | 10 |

### Communication and client-facing skills

| Evidence | Score range |
|---|---|
| No communication duties mentioned anywhere | 2–3 |
| Internal team collaboration mentioned | 4–5 |
| Self-assessed language level only (e.g. "upper-intermediate English") | 5–6 |
| Client communication listed as an explicit duty | 6–7 |
| External stakeholder management, presentations, or training delivery | 8–9 |
| Senior external communication (board-level, enterprise clients, public speaking) | 10 |

Do not score soft skills above 6 based on self-assessment alone.

### Soft skills *(problem-solving, attention to detail, adaptability)*
Only score these if directly evidenced by specific duties or outcomes — not assumed. Never score above 6 from self-assessment ("excellent problem-solver" = 5 maximum without supporting evidence).

---

## Experience Level Fit

Compare the JD's stated seniority against the candidate's total years of directly relevant experience and their most recent role title.

| JD Level | Ideal range | Score 9–10 | Score 6–8 | Score 3–5 | Score 1–2 |
|---|---|---|---|---|---|
| Trainee / Graduate | 0–1 yr | 0–1 yr relevant | 1–2 yr (slightly over) | 0 yr (no exp) | No relevant degree or exp |
| Junior | 1–3 yr | 1–3 yr | 0–1 or 3–4 yr | 4–6 yr (over) | No relevant exp |
| Mid-level | 2–5 yr | 2–5 yr | 1–2 or 5–6 yr | 6–8 yr (over) | < 1 yr |
| Senior | 5–10 yr | 5–10 yr | 3–5 yr | 10+ yr (over) | < 3 yr |
| Lead / Principal | 8+ yr | 8–15 yr | 5–8 yr | < 5 yr | No leadership evidence |

**Note:** Score lower when significantly overqualified — this reflects retention risk, not a quality judgment.

---

## Communication / Presentation
*(assessed from how the resume itself is written and structured)*

| Observation | Score |
|---|---|
| Polished structure, quantified achievements, precise language, no errors | 9–10 |
| Well-organised, clear descriptions, minor imprecision | 7–8 |
| Reasonable structure, some vague descriptions, limited quantification | 5–6 |
| Basic structure, mostly duty lists without context, some typos | 3–4 |
| Poorly formatted, hard to parse, significant errors, or extremely sparse | 1–2 |

Do not penalise non-native English speakers for phrasing style — penalise only for clarity issues that would affect professional communication.

---

## Overall Match Score — weighted formula

| Category | Weight |
|---|---|
| Must-Have Skills Coverage | **40%** |
| Responsibility Match | **25%** |
| Nice-to-Have Skills Coverage | **15%** |
| Experience Level Fit | **12%** |
| Communication / Presentation | **8%** |

```
Overall = (Must-Have avg × 0.40) + (Responsibility avg × 0.25) + (Nice-to-Have avg × 0.15) + (Experience × 0.12) + (Communication × 0.08)
```

Round to one decimal place.

**Responsibility Match conversion (for averaging):**
- Strong = 9
- Partial = 6
- Weak = 3

---

## Recommendation thresholds (HR Mode only)

| Tier | Condition |
|---|---|
| ✅ Recommend for Interview | Overall ≥ 7.0 AND Must-Have avg ≥ 7.0 |
| ⚠️ Recommend with Reservations | Overall 5.0–6.9 OR Must-Have avg 5.0–6.9 |
| ❌ Do Not Recommend | Overall < 5.0 OR Must-Have avg < 5.0 |

Must-Have avg is a **hard gate**. Overall 7.5 + Must-Have avg 4.8 = ❌.

---

## Spider chart axis grouping

When the JD lists more than 8 must-have skills, group related skills into single axes:

| Group | What goes in it |
|---|---|
| **Programming Languages** | All coding languages listed as must-have |
| **Infrastructure / DevOps** | OS, cloud, containerisation, CI/CD |
| **API & Connectivity** | Protocols, API types, integration tools |
| **Database Skills** | All database technologies |
| **Domain Knowledge** | Industry-specific knowledge items |
| **Communication** | Language proficiency, client-facing, presentation skills |
| **Analytical Skills** | Problem-solving, attention to detail, data analysis |

Grouped axis score = average of individual grouped scores, rounded to nearest integer. Always label grouped axes clearly on the chart.

---

## Edge cases

**Resume with no skills section**
Score based entirely on job duty descriptions. Cap all technical scores at 8 unless duties use explicit expertise language.

**Very short resume (under 1 page)**
Score what is there. Do not penalise for brevity in technical scores — only in Communication / Presentation if brevity makes the document unclear.

**Career change candidates**
Score domain knowledge low (1–3) when pivoting from an unrelated field. Score transferable technical skills normally based on evidence.

**Academic / research resumes**
Publications and research count as domain knowledge evidence. Academic projects count as project experience — cap technical scores from projects at 7 unless the project was industry-scale or published.

**Employment gaps**
Do not reduce technical skill scores for employment gaps unless the gap is 3+ years AND the technology has evolved significantly in that time. If reducing for this reason, state it explicitly in the Evidence column.

**Self-taught / bootcamp candidates**
Personal projects and open source contributions count as evidence. Score them one tier below equivalent professional experience (a personal project demonstrating a skill caps at 6; a professional role using the same skill caps at 10).