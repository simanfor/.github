# Text Formatting

## Bold, Italic and Inline Code

Use `**bold**` for file names, folder names, and document titles in content listings. Use `*italic*` for the language-switch link and for scientific species names.

```markdown
* **espanol**: contiene las fichas de los modelos en español
* **english**: contiene las fichas de los modelos en inglés

*[English version here](./README_english.md)*

masas irregulares de rebollo (*Quercus pyrenaica*)
```

Other available styles:

```markdown
**_Bold and italic_**

~~Strikethrough~~

`Inline code`
```

---

## Horizontal Rules and Line Breaks

Use `---` as a section divider throughout the document. Use two trailing spaces at the end of a line to force a line break within a paragraph.

```markdown
🇪🇸 **Estas viendo el contenido del repositorio en español**  

🇬🇧 *[English version here](./README_english.md)*

---
```

---

## Headings (Levels)

To keep document structure clean and consistent, use a **maximum of three heading levels** (`#`, `##`, `###`):

- `#` (H1): Reserved for the main document title (only one per document).
- `##` (H2): Used for main sections (e.g., `## 📜 Contenido`, `## ℹ️ Más información`).
- `###` (H3): Used for subsections under main sections.

Do **not** use `####` (H4) or deeper heading levels. If further nesting or sub-organization is required, use list formatting (`*`) or bold inline text (`**bold**`) instead.

---

## Language Header Pattern

Each repository has `README.md` (Spanish, main) and `README_english.md` (English) at its root. Both files start with a language-switch block immediately after the first `---`.

Spanish (`README.md`):

```markdown
# Título del repositorio

![simanfor](https://raw.githubusercontent.com/simanfor/web/main/logos/simanfor.png)

---

🇪🇸 **Estas viendo el contenido del repositorio en español**  

🇬🇧 *[English version here](./README_english.md)*

---
```

English (`README_english.md`), invert flags and link:

```markdown
🇬🇧 **You are viewing the content of the repository in English**

🇪🇸 *[Versión en español aquí](./README.md)*
```

---

## Emojis

SIMANFOR docs use **Unicode emoji only** — no GitHub shortcodes (`:emoji_name:`). Unicode renders consistently across GitHub, editors and PDF exports.

Section headers:

```markdown
## 🔗 Más contenidos de SIMANFOR en GitHub
## 🎬 Vídeos introductorios al uso de SIMANFOR
## 💾 Repositorios de trabajos donde se ha utilizado SIMANFOR
## ✏️ Cómo citar SIMANFOR
## 💻 Lista de contribuidores
## 📧 Contacto
## ℹ️ Más información
```

Content listing and list prefixes:

```markdown
📂  📖  🔢  🎯  🌳  🌲  📁
📜  ▶️  📚  📊  🔨  🇪🇸  🇬🇧
```

See [emoji.md](emoji.md) for the full mapping and usage rules.

---

## HTML Inline

Use HTML only for contributor profile pictures (badge-style avatars in the contributors section). Avoid it for logos and general content — use standard Markdown image syntax instead.

Contributor avatar (50 px):

```markdown
[![](https://github.com/aitorvv.png?size=50)](https://github.com/aitorvv)
```

---

## Blockquotes

```markdown
> Blockquote text.
> Multiple lines in the same blockquote.
```

---

## Table of Contents (Index)

For long files (those with multiple main sections or extensive scrolling), always include a **Table of Contents** (index) below the main title (or below the language switch header) to facilitate navigation.

Use standard Markdown list syntax with local anchor links pointing to the header titles:

```markdown
## Table of Contents

- [Overview](#overview)
- [When to Use](#when-to-use)
- [Best Practices](#best-practices)
```

### GitHub Flavored Markdown (GFM) Anchor Rules:
1. **Lowercase**: Convert all characters to lowercase (e.g., `## Best Practices` becomes `#best-practices`).
2. **Hyphens**: Replace spaces with hyphens `-`.
3. **Special characters**: Remove punctuation, emojis, and non-alphanumeric characters (e.g., `## ℹ️ Más información` becomes `#más-información`, ignoring the emoji symbol and leading/trailing spaces).

