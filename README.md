# Carnets

Site Hugo (thème `livre`) : journal, notes de lecture, dictionnaires, anthologie, citations.

Publié par GitHub Actions sur <https://vvnt.github.io/carnets/> à chaque push sur `main`.

## En local

```
hugo server
```

Build complet avec recherche :

```
hugo --gc --minify
npx pagefind --site public
```

## Conventions de contenu

- `content/journal/AAAA_MM_JJ.md` : une note par bloc, séparées par une ligne `---`.
  Si le fichier commence par une liste (`- …`), le faire précéder d'un front matter vide (`---` / `---`).
- `content/ndl/*.md` : front matter `title`, `author` (+ `subtitle`, `abstract`, `tags`).
- `content/dictionnaires/*.md` : un `# Lettre` par lettre, entrées `terme` / `: définition`.
- `content/anthologie.md` : `## Auteur`, `### Poème`.
- `content/citations.md` : citations séparées par `---`.
