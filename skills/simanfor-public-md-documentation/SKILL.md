---
name: simanfor-public-md-documentation
description: >
  SIMANFOR documentation for public repositories in markdown formatting, GitHub Flavored Markdown, README files, and documentation formatting. Use when writing SIMANFOR-related markdown docs, READMEs, or formatting documentation.
---

# Markdown Documentation for SIMANFOR

## Table of Contents

- [Overview](#overview)
- [When to Use](#when-to-use)
- [Templates](#templates)
- [Reference Guides](#reference-guides)
- [Best Practices](#best-practices)

## Overview

Conventions and patterns for creating well-formatted, consistent documentation across all SIMANFOR public repositories, using standard Markdown and GitHub Flavored Markdown (GFM).

## When to Use

- Writing or updating a `README.md` in any SIMANFOR repository
- Writing or updating a `README_english.md` in any SIMANFOR repository
- Updating shared content in `more_info_spanish.md` or `more_info_english.md`
- Adding a new contributor entry
- Formatting a citation block

---

## Templates

Ready-to-use starting points in the `templates/` directory:

| Template                                                        | Use for                   |
|-----------------------------------------------------------------|---------------------------|
| [doc-template_spanish.md](templates/doc-template_spanish.md)   | Spanish `README.md`       |
| [doc-template_english.md](templates/doc-template_english.md)   | English `README_english.md` |

Shared content (videos, repos, citation, contributors, license) lives in:

| File                                                                                                          | Language |
|---------------------------------------------------------------------------------------------------------------|----------|
| [more_info_spanish.md](https://github.com/simanfor/.github/blob/main/docs/more_info_spanish.md)               | Spanish  |
| [more_info_english.md](https://github.com/simanfor/.github/blob/main/docs/more_info_english.md)               | English  |

---

## Reference Guides

Detailed patterns in the `references/` directory:

| Guide                                                    | Contents                                                        |
|----------------------------------------------------------|-----------------------------------------------------------------|
| [text-formatting.md](references/text-formatting.md)     | Bold, italic, language header, emoji, HTML inline, blockquotes  |
| [lists.md](references/lists.md)                         | Two list styles: content listing and standard list              |
| [links-and-images.md](references/links-and-images.md)   | Links, images, absolute URLs, badge-style image links           |
| [emoji.md](references/emoji.md)                         | Unicode emoji only — section headers, list prefixes, flags      |
| [badges.md](references/badges.md)                       | Shields.io badge patterns for contributor profiles and license  |
| [contributors.md](references/contributors.md)           | Full contributor entry pattern with copy-paste ready blocks     |
| [citation.md](references/citation.md)                   | Plain-text citation and BibTeX block pattern                    |
| [code-blocks.md](references/code-blocks.md)             | Fenced code blocks and language specifiers                      |
| [tables.md](references/tables.md)                       | Table syntax for skill reference files                          |

---

## Best Practices

### ✅ DO

- Use descriptive link text — never "click here"
- Use absolute `raw.githubusercontent.com` URLs for images shared across repos
- Use `./README.md` for the Spanish link in `README_english.md` (both files are at root)
- Use two trailing spaces for line breaks within a paragraph
- Use `---` as a section divider
- Use Unicode emoji only — no GitHub shortcodes (`:emoji_name:`)
- Use standard Markdown `![alt](url)` for logos — no HTML `<img>` tags
- Add the two logos at the bottom of every README and more_info file
- Keep content-specific information in the README; put shared info in `more_info`

### ❌ DON'T

- Use HTML except for contributor avatar badges (50 px `[![](user.png)](profile)`)
- Break a Markdown link across two lines (`[text]` on one line, `(url)` on the next)
- Use relative paths for images that may be included from multiple repos
- Use GitHub emoji shortcodes (`:link:`, `:movie_camera:`, etc.) — use Unicode instead
- Commit `.Rhistory` or `.RData` files
