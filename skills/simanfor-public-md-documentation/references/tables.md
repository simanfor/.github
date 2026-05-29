# Tables

Tables in SIMANFOR docs appear in skill reference files (like this one), not in public-facing READMEs. Use them to summarise structured information such as badge availability or file catalogues.

Align column separators in source so the raw Markdown is readable in PR diffs and code review.

---

## Standard table

```markdown
| Guide                   | Contents                              |
|-------------------------|---------------------------------------|
| text-formatting.md      | Bold, italic, emoji, HTML inline      |
| lists.md                | Two list styles used in SIMANFOR      |
| links-and-images.md     | Links, images, absolute URLs, badges  |
```

## Aligned columns with centred cells

```markdown
| Contributor           | ORCID | LinkedIn |  X  |
|-----------------------|:-----:|:--------:|:---:|
| Felipe Bravo          |   ✓   |    ✓     |  ✓  |
| Aitor Vázquez         |   ✓   |    ✓     |  ✓  |
| Spyridon Michalakopoulos |  ✓   |    ✓     |     |
```

> `:---:` centres. `---:` right-aligns. `---` or `:---` left-aligns (default).

---

## Rules

* Pad cells with spaces so `|` separators align vertically across all rows.
* The separator row (`|---|`) must match the number of columns exactly.
* Do not use `<table>` HTML — pipe tables render identically on GitHub and are easier to diff.
