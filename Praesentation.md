% Praesentation in Markdown
% Referent: Tjorben Stihl
% Date: \today
---
theme: "AnnAbor"
header-includes:
colorrheme: "seahorse"
fronttheme: "structurebold"
---

# Erste Folie
Dies ist eine in Markdown erstellte Präsentation & als PDF.
````bash
pandoc -t beamer <filname.md> -o <praesentationname>.pdf
````

# Aufzählung mit Formattierung 

- punkt 1 mit *kursirves Text*
- punkt 2 mit **Fettem text**
- punkt 3 mit ~~Durchgestrichenem Text~~

# Formel und Quoting 

> **Merke**
Markdown ist kake

$$ \int_a \limits ^\infty \frac{x^2-a }{e^{x-b}}
dx$$

# Bilder einblenden

