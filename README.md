Les concepts-clés à propos des méthodes itératives et incrémentales de développement que sont TDD, ATDD et BDD sont (ou seront) réunis sur [StarDD.chrysocode.io](https://stardd.chrysocode.io/).

-- Xavier Pigeon

# Considérations Générales

## Espace du problème vs espace de la solution

En environnement complexe, il n'y a plus une solution pour un problème, mais une multitude de solutions possibles. Et bien souvent, le problème reste à découvrir, à questionner. Redéfinir le problème d'origine dans un cadre différent ouvre de nouvelles perspectives et permet d'envisager des solutions novatrices. Formuler des hypothèses pour explorer des solutions potentielles, c'est se donner des chances de découvrir une meilleure solution, voire de relever un défi qui paraissait insurmontable au départ.

Comment se positionner soi-même, un collègue ou des collaborateurs au sujet des métiers dans le développement de logiciels, en faisant abstraction des titres de postes, des diplômes, des textes de loi et conventions collectives, pour se focaliser seulement sur les aptitudes réelles ou une situation professionnelle donnée ?

![Ingénieur Logiciel vs Développeur](ressources/schemas/ingénieur_logiciel_vs_développeur.png)

Ingénieur logiciel | Développeur
------------------ | ------------
découvrir/questionner le problème | comprendre le problème posé
redéfinir le cadre du problème |
découper le problème | identifier des tâches
formuler des hypothèses |
explorer des solutions | trouver une solution
prouver et simplifier sa solution | vérifier sa solution

## Faut-il se former à TDD dès le début de sa carrière ?

Quand on se forme à un langage de programmation, on écrit généralement des morceaux de code pour réaliser de toutes petites tâches, comme autant d'exercices. On a donc le choix de vérifier le résultat soit en l'affichant en console (test manuel), soit en le testant en utilisant un framework de test (test automatisé). La deuxième option est bien meilleure, car on développe deux compétences conjointement au lieu d'une, car on apprend plus vite en maîtrisant ce qu'on fait, car automatiser ses tests n'est plus un sujet tabou. Ensuite, analyser un problème en sous-problèmes et commencer à définir un sous-problème en le décrivant sous la forme d'un test automatisé, tout cela avant de foncer tête baissée dans la recherche d'une solution, c'est déjà pratiquer TDD.

Au final, viser TDD même en commençant par des petits tests automatisés sur des petits morceaux de code est à mon avis la meilleure façon d'apprendre un langage de programmation, qu'on soit junior ou sénior d'ailleurs. On peut voir fleurir beaucoup de billets ou d'articles pour dissuader les juniors de s'intéresser à TDD dès le début... Plus tôt vous adopterez cette gymnastique de l'esprit, moins vous devrez désapprendre pour réapprendre, plus vite TDD sera une évidence, la vôtre.

# Test-Driven Development (TDD)

## Rouge-Vert-Remaniement avec le mantra de TDD

Mantra de TDD : "Tout code est coupable jusqu'à preuve de son innocence."

![TDD: Red-Green-Refactor](ressources/schemas/tdd_red_green_refactor.png)

## Les trois lois de TDD

Loi | Formulation correcte en français et sans ambiguïté
:-: | --------------------------------------------------
1   | Écris un test qui échoue avant d’écrire le code de production correspondant.
2   | Écris une seule assertion à la fois, qui fait échouer le test ou qui échoue à la compilation.
3   | Écris le minimum de code de production pour que l'assertion du test actuellement en échec soit satisfaite.

**NB :** Ces trois lois ne couvrent que les conditions à respecter en TDD pour arriver à un test qui réussit, en exprimant le minimalisme attendu du test en échec.

## Processus cyclique de TDD

Le micro-cycle de TDD se divise en deux nano-cycles : un nano-cycle de *Code-Driven Testing*, puis un nano-cycle de remaniement. C'est un processus itératif qui comporte cinq étapes.

Étape | Consigne
:---: | --------
1     | Écris un seul test qui décrit une partie du problème à résoudre.
2     | Vérifie que le test échoue, autrement dit qu'il est valide, c'est-à-dire que le code se rapportant à ce test n'existe pas.
3     | Écris juste assez de code pour que le test réussisse.
4     | Vérifie que le test passe, ainsi que les autres tests existants.
5     | Remanie le code, c'est-à-dire améliore-le sans en altérer le comportement, qu'il s'agisse du code de production ou du code de test.

![Micro-cycle et nano-cycles de TDD](ressources/schemas/cycle-global-tdd.png)

## TDD, ses pratiques et extensions

- Pratiques de TDD
  - *Code-Driven Testing*
  - Remaniement de code
- Pratiques dérivées de TDD
  - *Bug-Driven Development*
  - *Continuous TDD*
  - *TDD As If You Meant It*
  - *Behavior-Driven Development* (BDD) dérive à la fois de TDD et d'ATDD (*Acceptance-Driven Development*).

![TDD : pratiques et extensions](ressources/schemas/tdd_inheritance.png)

---
Contenus sous copyright et sous licence Creative Commons (CC), promus par [CHRYSOCODE](https://chrysocode.io/)