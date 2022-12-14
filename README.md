## Projet de livret de Vêpres à l'attention des fidèles

### Environnement de développement
- Pour Windows : télécharger et installer la distribution [TexLive](https://tug.org/texlive/windows.html)   
- Pour Mac, télécharger et installer la distribution [MacTeX](https://tug.org/mactex/mactex-download.html)   

Dans les deux cas, Gregorio fait déjà parti de la distribution, inutile de l'installer en plus.   
Bien suivre les tutos d'installations. Sur Windows, il n'y a rien à faire de plus, mais pour Mac, il est possible qu'il faille soit basculer le shell par défaut sur Bash avec la commande `chsh -s /bin/bash`, ou ajouter le le chemin de l'exécutable à la variable d'environnement $PATH du shell actif.

Il est fortement conseiller d'utiliser un IDE. [VSCode](https://code.visualstudio.com/download) dispose d'une extension dédiée, [LaTeX-Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop), qui permet de compiler les fichiers à chaque sauvegarde et d'ouvrir une fenêtre de prévisualisation (en plus des fonctionnalités courantes d'un IDE, syntaxe highlighting, autocomplétion, documentation, etc...)

### Développement
- Les fichiers `gabc` des antiennes, hymnes, etc, sont tirés de [Gregobase](https://gregobase.selapa.net/)       
- Pour les psaumes, utiliser l'outil [Chant Tools](https://bbloomf.github.io/jgabc/psalmtone.html) pour extraire le code gabc du premier verset, et le code tex pour les versets suivants :   
      * En haut à droite, choisir le psaume   
      * En haut à gauche, choisir le ton et la variante. Éventuellement, on peut choisir la clé. Ne pas toucher aux autres réglages.   
      * Juste en dessous à gauche, choisir `tex` pour le format des versets, cocher la cases `GABC for first verse`, et laisser le reste tel quel.   
      * Au milieu, le cadre GABC contient le code `gabc` du premier verset, à copier/coller dans un nouveau fichier `gabc` dans le dossier correspondant.   
      * Enfin, dans le dernier cadre se trouve le rendu du premier verset, ainsi que le code `tex` des versets suivants. Copier/coller le code tex dans le fichier adéquat.   

### Pour contribuer
- Créer une branche depuis `master`   
- Travailler sur cette branche et pousser les commits   
- Créer une PR vers `master`   
- La PR sera mergée sur `master` après validation   