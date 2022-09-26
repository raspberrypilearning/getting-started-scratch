## Déboguer

**Déboguer** consiste à trouver et à corriger des erreurs dans ton code qui sont appelées des **bogues**.

* Il est plus facile d'identifier les problèmes si tu effectues une modification à la fois, puis exécutes ton programme

* Il faudra peut-être plusieurs tentatives pour que ton projet fonctionne comme tu l'avais prévu

Voici quelques conseils qui peuvent t'aider à déboguer un projet lorsqu'il ne fait pas ce que tu veux qu'il fasse :

--- collapse ---
---
title: Exécuter de plus petits morceaux de code
---

Tu n'as pas besoin d'exécuter tout un programme pour vérifier si les derniers nouveaux blocs que tu as ajoutés fonctionnent.

* Clique sur un bloc dans la zone Code pour l'exécuter - c'est un moyen rapide de vérifier qu'un bloc fonctionne comme tu l'attends

* Pour tester un ensemble de blocs par eux-mêmes, fais-les glisser hors de leur script **contenant**, clique dessus pour les tester, puis fais-les glisser vers le script principal

--- /collapse ---

--- collapse ---
---
title: Ajouter des délais temporaires
---

Ralentis **l'exécution** de ton code lors de son exécution. Pour ce faire, ajoute un bloc `attendre`{:class="block3control"} ou `attendre jusqu'à ce qu'une touche soit pressée`{:class="block3control"}, puis supprime le bloc lorsque tu as fini de déboguer ton code.

--- /collapse ---

--- collapse ---
---
title: Afficher les variables sur la Scène
---

Si ton projet utilise des `variables`{:class="block3variables"} pour stocker des données, il peut être utile d'afficher ces `variables`{:class="block3variables"} sur la scène.

Clique sur la case à cocher à côté d'une `variable`{:class="block3variables"} dans la catégorie `Variables`{:class="block3variables"} pour l'afficher ou la masquer sur la scène.

La variable a-t-elle toujours la valeur que tu attends ?

--- /collapse ---

--- collapse ---
---
title: Ajouter des commentaires
---

Ajoute des commentaires aux blocs, aux ensembles de blocs et/ou aux scripts. Utilise un langage courant pour expliquer ce que fait le code. Parfois, cela te fera réaliser que ton code ne fait pas réellement ce que tu veux qu'il fasse !

Les commentaires sont utiles lorsque tu souhaites comprendre ton code plus tard, et ils aident d'autres personnes à comprendre tes projets.

--- /collapse ---


Il existe des problèmes communs que de nombreux débutants (et experts !) rencontrent avec Scratch.

--- collapse ---
---
title: Conseils de débogage pour des problèmes spécifiques
---

+ **Mon sprite se déplace à l'envers** — Ajoute un bloc `fixer le sens de rotation gauche-droite`{:class="block3motion"} ou un bloc `fixer le sens de rotation ne tourne pas`{:class="block3motion"}.

+ **Mon sprite « saute » lorsqu'il change de costume ou rebondit** — Assure-toi que le costume est centré dans l'éditeur graphique (aligne la croix bleue du costume avec le réticule au centre de l'éditeur graphique).

+ **Mon sprite s'arrête lorsqu'il atteint le bord de la Scène** — Ajoute un bloc `rebondir si le bord est atteint`{:class="block3motion"}.

+ **Mon son ne joue pas** — As-tu ajouté un bloc `jouer le son`{:class="block3sound"} lorsque l'on clique sur le sprite ? Si tu as copié le code d'un autre sprite, tu devras ajouter le son à ce sprite dans l'onglet **Sons**. Vérifie le volume sur ton ordinateur ou ta tablette et assure-toi que tu n'as pas baissé le volume avec le code — essaye `mettre le volume à`{:class="block3sound"} `100`.

+ **D'autres sprites passent devant mon sprite** — Utilise un bloc `aller à l'avant-plan`{:class="block3looks"}.

+ **Mon sprite ne bouge/ne change qu'une seule fois** — Mets ton code dans un bloc `répéter indéfiniment`{:class="block3control"} afin qu'il continue de s'exécuter.

+ **Mon sprite ne change pas lorsque je déplace un curseur variable** — Place ton code dans un bloc `répéter indéfiniment`{:class="block3control"} afin qu'il continue de se mettre à jour.

--- /collapse ---

**Astuce :** Si tu ne trouves pas le problème après avoir essayé ces techniques, fais une pause ou travaille sur une autre partie de ton projet. À ton retour, tu pourrais trouver le bogue tout de suite !

