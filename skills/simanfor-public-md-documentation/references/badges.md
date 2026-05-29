# Badges

Badges in SIMANFOR docs are always `[![label](shields-url)](target-url)` image-links rendered inline. They appear in two contexts: contributor profiles and the license section.

---

## Contributor profile badges

Each badge links to the contributor's external profile. Place each badge on its own line with a trailing space so they render in a horizontal row.

### Academic / professional networks

```markdown
[![ORCID](https://img.shields.io/badge/ORCID-green?logo=orcid)](https://orcid.org/XXXX-XXXX-XXXX-XXXX) 
[![ResearchGate](https://img.shields.io/badge/ResearchGate-00CCBB?logo=researchgate&logoColor=white)](https://www.researchgate.net/profile/PROFILE) 
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-4285F4?logo=google-scholar&logoColor=white)](https://scholar.google.com/citations?user=ID) 
```

### Social / contact

```markdown
[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:name@uva.es)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/PROFILE) 
[![X](https://img.shields.io/badge/X-1DA1F2?logo=x&logoColor=white)](https://twitter.com/HANDLE) 
```

### Institution logo (UVa — uses `<img>` exception)

```markdown
[<img src="https://raw.githubusercontent.com/aitorvv/aitorvv/main/logos/uva.jpg" alt="UVa" width="22">](https://portaldelaciencia.uva.es/investigadores/ID/detalle)
```

### Badge availability by contributor

| Contributor | Email | ORCID | Scholar | ResearchGate | LinkedIn | X | UVa |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Felipe Bravo | — | ✓ | — | ✓ | ✓ | ✓ | ✓ |
| Cristóbal Ordóñez | — | ✓ | — | ✓ | ✓ | ✓ | ✓ |
| Aitor Vázquez | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Spyridon Michalakopoulos | — | ✓ | — | ✓ | ✓ | ✓ | ✓ |

---

## License badge

Placed at the start of the license section, links to the `./LICENSE` file:

```markdown
[![MIT License](https://img.shields.io/badge/license-MIT-red.svg)](./LICENSE)
```
