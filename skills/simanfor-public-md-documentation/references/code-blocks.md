# Code Blocks

Always use fenced code blocks with a language specifier. This enables syntax highlighting on GitHub and most Markdown previewers.

---

## Bash / shell commands

Used in Docker and setup documentation for commands the user must run.

````markdown
```bash
docker pull simanfor/simanfor:latest
docker run -v /path/to/data:/data simanfor/simanfor:latest
```
````

For single-line commands or terminal output, also use `bash`:

````markdown
```bash
pip install -r requirements.txt
```
````

---

## Python

Used for script examples or configuration snippets.

````markdown
```python
import pandas as pd

df = pd.read_csv("inventory.csv")
print(df.head())
```
````

---

## BibTeX

Used for the citation entry in the English `more_info` file.

````markdown
```bibtex
@article{bravo_simanfor_2025,
	title = {{SIMANFOR} cloud {Decision} {Support} {System}: {Structure}, content, and applications},
	volume = {499},
	issn = {0304-3800},
	doi = {10.1016/j.ecolmodel.2024.110912},
	journal = {Ecological Modelling},
	author = {Bravo, F. and Ordóñez, C. and Vázquez-Veloso, A. and Michalakopoulos, S.},
	year = {2025},
	pages = {110912},
}
```
````

---

## Markdown (for skill reference files)

Used in this skill's own reference files to show Markdown examples.

````markdown
```markdown
content here
```
````

---

## Language specifier reference

| Specifier | Use for |
|---|---|
| `bash` | Shell commands, Docker commands, terminal output |
| `python` | Python scripts and snippets |
| `bibtex` | Citation entries |
| `markdown` | Markdown examples (in skill reference files) |
| `dockerfile` | Dockerfile content |
