# DS5020 Mini-Project 02 — Will This Be a Strong Sales Week?

Bayes' theorem and Naive Bayes on the Walmart weekly sales dataset
(45 stores × 143 weeks, February 2010 – October 2012).

| Role | Name | Owns |
|------|------|------|
| Data Analyst | Muhammad Saad Malik | Warm-up (W1–W7), Part P, Part B |
| ML Engineer | Jagadeesh Aravind Kalyan Shetti | Part N |
| Both | Muhammad Saad Malik & Jagadeesh Aravind Kalyan Shetti | J1 note, final "Restart & Run All" check |

## Layout

```
.
├── data/
│   ├── README.md              # how to download Walmart.csv (the CSV itself is git-ignored)
│   └── Walmart.csv            # this is where the data should be stored
├── notebooks/
│   └── walmart_bayes.ipynb   
├── figures/                   # saved plots (store numbers only, R4)
├── submission/
│   ├── answer_sheet.md        # Section 7, filled in
│   └── note.txt               # J1: 5 sentences to Maria
├── requirements.txt
└── README.md
```

## Setup

```bash
python -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Then get the data (see `data/README.md`) and run:

```bash
jupyter lab notebooks/miniproject02_walmart_bayes.ipynb
```

## Working together with git

- `git pull` before you start, commit small, `git push` when you stop.
- A notebook is one big JSON file, so two people editing it at once causes painful merge conflicts. Agree who has the notebook "checked out" at any moment, or each work on a branch (`part-pb`, `part-n`) touching only your own sections, and merge one branch at a time.
- Before every commit: *Kernel → Restart & Run All*, so the saved outputs match the code.
- Optional: `pip install nbdime && nbdime config-git --enable` gives readable notebook diffs and merges.

## Rules checklist

- [ ] R1 Event definitions written before any computation (Section 1 of the notebook)
- [ ] R2 One row = one store-week; sample space = 6,435 store-weeks
- [ ] R3 Train 2010–2011, test 2012; store averages from training weeks only
- [ ] R4 Store numbers only in the note and figures
- [ ] R5 Every reported probability checked a second way

## Submission checklist

- [ ] Notebook runs top to bottom with no errors
- [ ] `submission/answer_sheet.md` filled in
- [ ] `submission/note.txt`: five plain sentences with numbers