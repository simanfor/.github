# Lists

SIMANFOR READMEs use two list styles. Use the correct one for the context — do not mix them.

---

## Style 1 — Content listing

For the `## 📜 Contenido` / `## 📜 Content` section: describes folders, files and documents. Each item uses `*`, a Unicode emoji, **bold name**, colon, and description.

```markdown
* 📂 **espanol**: contiene las fichas de los modelos en español
* 📖 **SIMANFOR_escenarios.pdf**: explicación del funcionamiento de los escenarios
* 🔢 **IFN4_codigos_especies.csv**: códigos de especies del IFN4
* 🎯 **corta**: breve explicación sobre la configuración de las cortas
```

Nested (subfolder contents — 4-space indent, same style):

```markdown
* 📂 **arbol_individual**: fichas descriptivas de modelos de árbol individual:
    * 🌳 para **masas puras**
    * 🌳🌲 para **masas mixtas**
```

---

## Style 2 — Standard list

For all other lists: cross-repository links, videos, publication and project repositories. Uses `*`, optional Unicode emoji prefix, and linked or plain text. Nested items use 4-space indent + `*`.

Cross-repository links (no emoji):

```markdown
* [Escenarios en SIMANFOR](https://github.com/simanfor/escenarios)
* [Introducción a SIMANFOR](https://github.com/simanfor/introduccion)
* [Inventarios en SIMANFOR](https://github.com/simanfor/inventarios)
* [Manual de uso de SIMANFOR](https://github.com/simanfor/manual)
* [Modelos en SIMANFOR](https://github.com/simanfor/modelos)
* [Publicaciones acerca de SIMANFOR](https://github.com/simanfor/publicaciones)
* [Resultados de simulación en SIMANFOR](https://github.com/simanfor/resultados)
* [Web de SIMANFOR](https://github.com/simanfor/web)
```

Video list (nested):

```markdown
* 📜 Lista de reproducción: [SIMANFOR: Sistema de apoyo...](https://youtube.com/playlist?list=PLsdzTKpJZZa7vn5zGpn07-bd0Nce-fMhJ&feature=shared)
    * ▶️ [Introducción a SIMANFOR](https://youtu.be/Y8pWcPdHsMY?feature=shared)
    * ▶️ [Documentación de SIMANFOR en GitHub](https://youtu.be/i4AXBrm4PqI?feature=shared)
    * ▶️ [Mi primera simulación en SIMANFOR](https://youtu.be/kCRNgIsfAn8?feature=shared)
```

Publication and project repositories:

```markdown
💾 📚 Repositorios asociados a publicaciones:
* 📚 [Repositorio con simulaciones de masas irregulares de rebollo (*Quercus pyrenaica*)](https://github.com/aitorvv/Quercus_pyrenaica_silviculture_CyL) para el artículo titulado **Dealing with complex forests...**

💾 🔨 Repositorios asociados a proyectos:
* 📊 [Repositorio con simulaciones para masas mixtas](https://github.com/iuFOR-QuantitativeForestry/COMFOR.NFI) del proyecto [COMFOR-SUDOE](https://www.comfor-sudoe.eu/es/)
```
