# Instrucciones para Agentes de IA en SIMANFOR

Este archivo recopila el contexto del espacio de trabajo de **SIMANFOR** y las directrices técnicas necesarias para que cualquier agente de IA (u otro desarrollador) pueda explorar, mantener y mejorar el contenido de este repositorio de forma segura y eficiente en el futuro.

---

## 🗺️ Estructura del Espacio de Trabajo

El espacio de trabajo principal es una colección de **11 repositorios independientes de GitHub** agrupados bajo una misma carpeta organizativa. Cada subcarpeta es un repositorio Git propio:

1. **`.github`**: Contiene configuraciones globales de la organización y el README del perfil de SIMANFOR.
2. **`introduccion`**: Materiales de introducción a la plataforma, vídeos explicativos y guías iniciales en PDF.
3. **`escenarios`**: Documentación y guías sobre cómo configurar escenarios selvícolas y actividades de manejo.
4. **`inventarios`**: Plantillas, códigos y archivos de ejemplo (CSV, PDF) para preparar datos de parcelas forestales para SIMANFOR.
5. **`manual`**: Manual de usuario completo de SIMANFOR.
6. **`modelos`**: Fichas descriptivas de los modelos de crecimiento y producción forestal integrados (árbol individual, masa, masas puras, mixtas, etc.).
7. **`resultados`**: Scripts de análisis de simulaciones en R (`Rmd`), informes de simulación automáticos y plantillas Excel.
8. **`web`**: Recursos y logos específicos utilizados en la interfaz y en los READMEs del simulador.
9. **`publicaciones`**: Archivo bibliográfico principal (`.bib`) y lista de referencias asociadas al proyecto.
10. **`docker`**: Repositorio con la documentación pública de usuarios para la ejecución del simulador en local mediante Docker.
11. **`privado`**: Contenido privado que incluye diapositivas, abstracts de congresos, docencia y material de trabajo preliminar.

---

## 🔍 Reglas de Calidad e Inspección

Cualquier trabajo futuro sobre este repositorio debe adherirse a los siguientes estándares de control de calidad:

### 1. ⚠️ Corrección de Enlaces Rotos y Renderizado de Markdown
* **Saltos de Línea en Enlaces**: Nunca uses saltos de línea entre el texto de la etiqueta `[...]` y su URL `(...)`. Por ejemplo:
  * ❌ *Incorrecto* (rompe el renderizado en GitHub):
    ```markdown
    [COMFOR-SUDOE]
    (https://www.comfor-sudoe.eu/es/)
    ```
  *  *Correcto*:
    ```markdown
    [COMFOR-SUDOE](https://www.comfor-sudoe.eu/es/)
    ```
* **Enlaces a Licencias**: Los archivos `README_english.md` residen en la raíz del repositorio junto con `README.md`. El enlace a la licencia desde ambos archivos es siempre `./LICENSE`.
* **Enlaces Absolutos vs. Relativos**: Para enlaces externos a internet, incluye siempre el protocolo completo (`https://` o `http://`). Si se omite (ej. `dx.doi.org`), los motores Markdown lo interpretarán como una ruta de archivo local rota.

### 2. ✍️ Pautas Ortográficas y Terminología
* **Revisión de Textos**: Los archivos de documentación se redactan de forma paralela en español (`README.md`, en la raíz) e inglés (`README_english.md`, también en la raíz del repositorio).
* **Palabras Clave Ignoradas**: Ciertos términos propios del ecosistema forestal y nombres de los autores no deben marcarse como faltas ortográficas (ej. `SIMANFOR`, `iuFOR`, `UVa`, `ETSIIAA`, `Felipe Bravo`, `Aitor Vázquez`, `LifeRebollo`, `CrossForest`, `IBERO`, `Rhistory`, `RData`, etc.).

### 3. 🧹 Archivos Innecesarios de R
* R genera archivos temporales e historiales locales (`.Rhistory` y `.RData`).
* **Regla**: Estos archivos **nunca** deben subirse a producción o guardarse en los repositorios de GitHub.
* **Acción**: Si encuentras archivos `.Rhistory` o `.RData`, elimínalos y asegúrate de que estén listados en el archivo `.gitignore` correspondiente.

---

## 🛠️ Flujo de Trabajo en Git

Al realizar modificaciones:
1. Dado que cada carpeta es un repositorio independiente, los commits y push deben hacerse **de forma individual dentro de cada subcarpeta**.
2. **Ejemplo de flujo de confirmación**:
   ```bash
   cd escenarios
   git add README.md
   git commit -m "docs: corregir enlaces y ortografía en README"
   git push origin main
   ```
3. No realices commits masivos globales que crucen repositorios a menos que sea estrictamente necesario.

---

![simanfor](https://raw.githubusercontent.com/simanfor/.github/main/skills/simanfor-public-md-documentation/resources/simanfor.png)

![SMART_GIR](https://raw.githubusercontent.com/simanfor/.github/main/skills/simanfor-public-md-documentation/resources/SMART_GIR.png)

