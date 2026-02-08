# academic-writing-refiner

A [Claude Skill](https://code.claude.com/docs/en/skills) for refining academic writing for computer science research papers targeting top-tier venues (NeurIPS, ICLR, ICML, AAAI, IJCAI, ACL, EMNLP, NAACL, CVPR, WWW, KDD, SIGIR, CIKM).

## What It Does

Transforms rough or intermediate academic drafts into polished, publication-ready prose. Focuses on **clarity and precision over fancy vocabulary** — the kind of writing that reviewers appreciate because it communicates ideas efficiently.

- **Full paper or single section refinement** with section-specific conventions
- **LaTeX-aware editing** — preserves `\cite{}`, `\ref{}`, equations, and macros
- **Venue-aware style** — adapts to ML, NLP, CV, and IR/Web community norms
- **Rebuttal writing** — guidance for crafting effective author responses
- **Light proofreading** mode for grammar-only fixes

## Installation

1. Download `academic-writing-refiner.skill` from this repo
2. Open [Claude Settings](https://claude.ai/settings) → **Skills** → **Add Skill**
3. Upload the `.skill` file

Alternatively, add the `academic-writing-refiner/` folder contents directly to `~/.claude/skills/` (All your projects) or `.claude/skills/` (This project only).

## Usage

You can start with:

```
Refine this introduction for my ICML submission by using the "academic-writing-refiner" skill: [paste text]
```
```
Help me write a rebuttal for these NeurIPS reviews by using the "academic-writing-refiner" skill: [paste comments]
```
```
Light edit only — just fix grammar via "academic-writing-refiner" skill: [paste text]
```

The output includes refined text (matching your input format), brief notes on substantive changes, and flagged issues it cannot fix.

## Structure

```
├── academic-writing-refiner.skill   # Installable skill package
└── academic-writing-refiner/
    ├── SKILL.md                     # Core instructions and refinement process
    └── references/
        ├── section-guide.md         # Conventions per section (abstract → conclusion)
        ├── rebuttal-guide.md        # Author response guide
        └── word-choice.md           # Word substitution quick reference
```

## Contributing

Contributions welcome — especially additional venue conventions (e.g., ICSE, CHI, OSDI), before/after examples, and expanded rebuttal templates. Fork, edit the relevant `.md` files, and submit a PR.

## License

[MIT](LICENSE)
