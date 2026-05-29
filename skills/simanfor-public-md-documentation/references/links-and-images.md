# Links and Images

---

## Standard links

Always use descriptive link text. Never use "click here".

```markdown
[SIMANFOR](https://www.simanfor.es)
[ficha](https://github.com/simanfor/modelos)
[licencia MIT](./LICENSE)
```

Each repository has two README files at its root:
- `README.md` — Spanish version (main)
- `README_english.md` — English version

Link from the English file back to Spanish:

```markdown
*[Versión en español aquí](./README.md)*
```

Link from the Spanish file to the English version:

```markdown
*[English version here](./README_english.md)*
```

---

## Images

Always use **absolute `raw.githubusercontent.com` URLs** for images referenced across repositories. This ensures they render correctly regardless of which repo includes the file.

Logos at the bottom of every README and more_info file:

```markdown
![simanfor](https://raw.githubusercontent.com/simanfor/.github/main/skills/simanfor-public-md-documentation/resources/simanfor.png)

![SMART_GIR](https://raw.githubusercontent.com/simanfor/.github/main/skills/simanfor-public-md-documentation/resources/SMART_GIR.png)
```

---

## Badge-style image links

Contributor avatar (50 px, links to GitHub profile):

```markdown
[![](https://github.com/aitorvv.png?size=50)](https://github.com/aitorvv)
```

Shields.io badges (link to external profile) — see [badges.md](./badges.md) for the full catalogue.

UVa institution logo (uses `<img>` tag to control size — accepted exception):

```markdown
[<img src="https://raw.githubusercontent.com/aitorvv/aitorvv/main/logos/uva.jpg" alt="UVa" width="22">](https://portaldelaciencia.uva.es/investigadores/178830/detalle)
```
