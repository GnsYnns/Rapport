# Projet LaTeX : Rapport Mission 4 : RSE et Numérique Responsable d'Iveco Group

## Structure du projet

```
Rapport/
├── main.tex                  % Fichier maître
├── sections/
│   ├── acronymes.tex         % Liste des sigles et acronymes
│   ├── entreprise.tex        % Présentation d'Iveco et du site de Haute-Goulaine
│   ├── introduction.tex      % Contexte et objectifs de la mission
│   ├── gouvernance.tex       % Partie 1 : Gouvernance et engagements globaux
│   ├── social.tex            % Partie 2 : DEI, santé-sécurité et communautés
│   ├── numerique.tex         % Partie 3 : Numérique responsable et recommandations
│   ├── conclusion.tex        % Conclusion
│   └── glossaire.tex         % Glossaire
├── bib/
│   └── references.bib        % Fichier bibliographique (BibLaTeX/Biber)
└── README.md                 % Ce fichier
```

## Compilation

Le projet utilise **BibLaTeX** avec le moteur **Biber**. La séquence de compilation recommandée est :

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

Si votre installation utilise `bibtex` à la place de `biber`, remplacez `biber main` par `bibtex main`.

## À personnaliser avant remise

Dans `main.tex` :

- `\MONNOM` : remplacer `[Nom Prénom]` par votre nom.
- `\MONECOLE` : remplacer `[Nom de l'école]` par votre école.
- `\NOMTUTEUR` : remplacer `[Nom du tuteur entreprise]` par le nom de votre tuteur.
- `\date{Juillet 2026}` : adapter la date si nécessaire.

## Conseils

- Vérifiez que `pdflatex`, `biber` et les packages listés dans `main.tex` sont installés.
- En cas d'erreur de police ou de package, lancez `tlmgr install <package>` (TeX Live) ou utilisez le gestionnaire de packages MiKTeX.
