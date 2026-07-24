## 1. CONTRAINTES DE LONGUEUR ET STRUCTURE GLOBALE

Le document LaTeX généré doit impérativement respecter la structure et la pagination suivantes :

* **Page de garde :** Titre, Nom, Entreprise (Iveco Group), Date, Tuteur.
* **Remerciements** (1 page max).
* **Sommaire / Table des matières** (généré automatiquement).
* **Liste des sigles et acronymes** (Tableau des marques/sigles).
* **Description de l'entreprise :** 3 pages maximum (Utilise Intro.tex dans Consigne - en modifiant :
-  régalienne : Adjectif non adapté à une entreprise. Parlez plutôt de services généraux de l'entreprise.
-  "Cela élimine le syndrome du « ça fonctionne sur ma machine mais pas sur le serveur », puisque mon environnement de dev local utilise le même noyau Linux que nos serveurs de production." : ça ne se dit pas à l'écrit ).
* **Thème de la mission :** Définition des objectifs et du contexte (Non comptabilisée dans les 10 pages).
* **Développement (Thème RSE & Numérique Responsable) :** **10 pages maximum** (Cœur du rapport).
* **Conclusion :** Bilan et perspectives (Non comptabilisée dans les 10 pages).
* **Glossaire :** Explication des termes techniques.
* **Bibliographie / Liste des sources :** Présentation académique.
* **Annexes :** Pour les éléments volumineux.

## 2. RÈGLES DE MISE EN PAGE ET TYPOGRAPHIE

* **Format de page :** A4 (`a4paper`).
* **Marges :** 2.5 cm de chaque côté (utiliser le package `geometry`).
* **Police et espacement :** Taille 11pt ou 12pt, interligne de 1.15 ou 1.5. Le texte doit être justifié.
* **Hiérarchie des titres :** Utiliser une numérotation claire (1., 1.1., 1.1.1.). Les titres doivent être mis en évidence (gras, taille supérieure) sans utiliser de soulignement.
* **Sauts de page :** Chaque grande partie (Description de l'entreprise, Introduction, Développement, Conclusion) doit commencer sur une nouvelle page (`\newpage` ou `\clearpage`).

## 3. TRAITEMENT DES SIGLES, ACRONYMES ET MARQUES

* **Liste des sigles :** Un tableau récapitulatif ou une liste générée automatiquement (via le package `acronym` ou `glossaries`) doit être présent au début du document.
* **Première utilisation dans le texte :**
* Le sigle doit être écrit en toutes lettres suivi de l'acronyme entre parenthèses.
* *Règle stricte :* Insérer une note de bas de page (`\footnote{}`) donnant la traduction française explicite si le sigle est d'origine étrangère (ex: *DEI (Diversity, Equity and Inclusion)* -> Note de bas de page : *Diversité, Équité et Inclusion*).


* **Utilisations suivantes :** Utiliser uniquement l'acronyme.

## 4. ANGLICISMES ET VOCABULAIRE ÉTRANGER

* **Italique obligatoire :** Tout mot étranger ou anglicisme (ex: *Green IT*, *Quick Win*, *Corporate Volunteering*, *Playbook*) doit systématiquement être mis en italique (`\textit{}`).
* **Traduction en note de bas de page :** Lors de la première apparition d'un anglicisme incontournable, ajouter une note de bas de page proposant l'équivalent français recommandé (ex: *Green IT* -> Note de bas de page : *Numérique éco-responsable*). Privilégier le français dans le texte lorsque l'alternative existe et est fluide.

## 5. GLOSSAIRE

* Créer une section "Glossaire" à la fin du document (avant la bibliographie).
* Y inclure tous les termes techniques, le jargon d'entreprise propre à Iveco Group, ou les concepts RSE complexes (ex: *Bilan Carbone*, *B4SI*, *Whistleblowing*).
* Les mots présents dans le glossaire doivent idéalement être signalés par un astérisque (*) lors de leur première occurrence dans le texte.

## 6. TRAITEMENT DES SOURCES ET BIBLIOGRAPHIE

* **Appels de citation dans le texte :** Chaque information chiffrée, KPI ou affirmation issue d'un document interne (ex: le chiffre de 4% de travailleurs en situation de handicap) doit faire l'objet d'une citation dans le texte (ex: `\cite{doc_DEI}`).
* **Format de la Bibliographie :** Utiliser un standard reconnu (APA ou IEEE) via `biblatex` ou `bibtex`.
* **Catégorisation des sources :** Séparer la bibliographie en sous-catégories si nécessaire (Documents internes Iveco Group, Sites Web, Articles académiques).
* Le listage doit comporter : Titre du document, Auteur/Entité (ex: Iveco Group), Date de publication (si disponible), et Type de document (ex: PDF interne, Page SharePoint).

## 7. ÉLÉMENTS GRAPHIQUES ET TABLEAUX

* **Numérotation et Légende :** Chaque figure (image, schéma) et chaque tableau doit posséder un numéro et une légende descriptive (`\caption{}`).
* **Centrage :** Tous les éléments graphiques doivent être centrés.
* **Référencement :** Le texte doit systématiquement faire référence à la figure ou au tableau avant qu'il n'apparaisse (ex : "Comme l'illustre la Figure 1...").
* Si une image ou un tableau est tiré d'une des ressources, la source doit être mentionnée dans la légende.

## 8. QUALITÉ DE RÉDACTION ET RÔLE DE L'IA

* **Orthographe et syntaxe :** Niveau de français irréprochable (tournures professionnelles, grammaire, orthographe).
* **Esprit de synthèse :** Utiliser des schémas commentés et des listes à puces pour éviter les longs blocs de texte indigestes, tout en conservant le niveau de détail attendu d'un ingénieur.
* Le code LaTeX généré ne doit comporter aucune erreur de compilation.