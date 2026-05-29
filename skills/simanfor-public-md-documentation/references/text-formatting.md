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
