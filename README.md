# ⚠️ Avertissement ⚠️
{: .no_toc }

Ce site est en cours de construction : ne soyez pas surpris si un paragraphe semble inachevé ou s'il est resté vide.

# Bienvenue dans le Monde de la Révolution Logicielle !
{: .no_toc }

Êtes-vous prêt à plonger au cœur de méthodes de développement qui peuvent révolutionner la manière dont les logiciels prennent vie ? Vous avez atterri sur le site ultime dédiée à la découverte, à la compréhension et à la maîtrise dans le domaine du développement logiciel piloté par le test. Que vous soyez un codeur chevronné, un testeur acharné ou simplement un esprit curieux, notre espace est conçu pour éveiller votre passion pour la création de logiciels de grande qualité.🏅🏆

Imaginez un endroit où le code prend vie avec une précision chirurgicale, où les fonctionnalités et algorithmes évoluent en harmonie avec les besoins des utilisateurs, et où chaque ligne de code est un pas de danse dans le ballet complexe de la conception logicielle. Bienvenue dans l'univers des méthodes itératives et incrémentales, TDD, ATDD et BDD -- trois méthodes puissantes qui transforment l'art du codage en une discipline précise, créative et collaborative.

Que vous soyez en quête de connaissances pour perfectionner votre art, ou que vous désiriez explorer ces méthodes sous un angle nouveau et innovant, vous êtes au bon endroit. Notre site regorge de ressources authentiques et détaillées, des concepts de base aux subtilités avancées, des diagrammes illustratifs aux études de cas réels. Tout cela dans le but de vous guider, vous inspirer et vous aider à élever vos compétences à un niveau supérieur.

Mais attendez, ce n'est pas tout. Ce site n'est pas seulement une source de savoir. C'est un hommage à la communauté dynamique des passionnés qui œuvrent sans relâche pour repousser les limites du possible dans le monde numérique. C'est un espace où 🔍 heuristique, 💡 créativité, 🤝 collaboration et 🔬 analyse fusionnent avec une vision holistique de la qualité logicielle pour créer une synergie qui transcende la programmation.🌟

En parcourant ces contenus, vous découvrirez également une voix, une expérience, une expertise : celle d'un passionné qui s'est immergé dans ces méthodes, les a pratiquées, les a affinées. Ce site est un témoignage vivant de l'engagement envers l'excellence, et il aspire à vous guider vers de nouveaux sommets dans votre propre parcours de développement.

Préparez-vous à vous immerger dans un voyage de découvertes. Préparez-vous à explorer les concepts, à démystifier les processus et à transformer votre manière de créer des logiciels. Que vous soyez ici pour apprendre, pour collaborer ou pour défier le statu quo, nous vous invitons à embarquer pour un voyage qui changera votre façon de penser la création logicielle.

Soyez prêt à repousser les limites, à embrasser le changement et à créer avec passion.

Bienvenue dans *Star-Driven Development*. Votre aventure commence maintenant !🚀✨


![Définitions de TDD, BDD et ATDD](ressources/schemas/tdd_atdd_bdd__definitions__fr.png)

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

- Table des matières
{:toc}

# Comment ces méthodes sont-elles devenues incontournables ?

Aujourd'hui, la question n'est plus du tout de savoir pourquoi il faudrait s'intéresser à ces méthodes, mais plutôt de comprendre ce qu'elles permettent de faire.

## Un monde complexe et ambigu

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

Face à la complexité, la simplicité est notre salut. Face à l'ambiguïté, sa complice, l'heuristique est notre meilleure alliée.

> La simplicité est la sophistication suprême. -- Léonard de Vinci

## Un monde volatile et incertain

# Test-Driven Development (TDD)

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

## Définition de TDD

TDD est une méthode incrémentale qui guide les développements par micro-cycles depuis l'analyse et le découpage du problème jusqu'à aboutir à une solution minimaliste, simple et prouvée, en faisant émerger la conception par empirisme, afin de livrer continuellement un produit toujours plus fiable aux utilisateurs.

## Rouge-Vert-Remaniement

> Tout code est coupable jusqu'à preuve de son innocence. -- Mantra de TDD

![TDD: Red-Green-Refactor](ressources/schemas/tdd_red_green_refactor.png)

- Rouge ! C'est un moment primordial de TDD, où nous nous projetons dans l'espace du problème.
- Vert ! C'est un moment central de TDD, où nous nous projetons dans l'espace de la solution.
- Remaniement ! C'est un moment charnière de TDD, où nous nous préparons déjà pour le prochain cycle.

## Pilliers de TDD

TDD repose sur cinq [pilliers][TDD Manifesto/Values] qui changent radicalement la manière de développer des logiciels.
1. Des petits pas plutôt que des changements de grande ampleur.
2. Un remaniement continuel plutôt que des améliorations tardives.
3. Une conception qui émerge au fil du temps plutôt qu'une conception globale en amont.
4. Une documentation exécutable plutôt que des documents statiques.
5. Un code minimaliste plutôt qu'une solution plaquée or.

## Les trois lois de TDD

Ces lois énoncent les conditions à respecter en TDD pour arriver à un test qui réussit, autrement dit pour passer du rouge au vert. Elles formalisent les trois étapes à dérouler chronologiquement quand on amorce un nouveau cycle de TDD.

Loi | Formulation correcte en français et sans ambiguïté
:-: | --------------------------------------------------
1   | Écris un test qui échoue avant d’écrire le code de production correspondant.
2   | Écris une seule assertion à la fois, qui fait échouer le test ou qui échoue à la compilation.
3   | Écris le minimum de code de production pour que l'assertion du test actuellement en échec soit satisfaite.

**NB :** Ces lois expriment le minimalisme attendu du test en échec, autant que du code de production.

## Processus cyclique de TDD

Le micro-cycle de TDD se divise en deux nano-cycles : un nano-cycle de *Code-Driven Testing*, puis un nano-cycle de remaniement. C'est un processus itératif qui comporte cinq étapes.

![Cycle global de TDD](ressources/schemas/tdd_global_cycle__fr__chrysocode.png)

Étape | Consigne
:---: | --------
1     | Écris un seul test qui décrit une partie du problème à résoudre.
2     | Vérifie que le test échoue, autrement dit qu'il est valide, c'est-à-dire que le code se rapportant à ce test n'existe pas.
3     | Écris juste assez de code pour que le test réussisse.
4     | Vérifie que le test passe, ainsi que les autres tests existants.
5     | Remanie le code, c'est-à-dire améliore-le sans en altérer le comportement, qu'il s'agisse du code de production ou du code de test.

## Pratiques et extensions de TDD

![TDD : pratiques et extensions](ressources/schemas/tdd_inheritance__fr.png)

- Pratiques strictement incluses : TDD implique de les utiliser.
  - *Code-Driven Testing*
  - Remaniement de code
- Pratiques additionnelles : elles ne modifient pas TDD, elles y greffent seulement quelques éléments.
  - *Continuous TDD*
  - *TDD As If You Meant It*
  - *Transformation Priority Premise*
- Méthodes dérivées : elles héritent de TDD, en respectant son cycle, et y apportent des changements.
  - *Bug-Driven Development*
  - *Documentation-Driven Development*
  - *Behavior-Driven Development* (BDD), qui dérive à la fois de TDD et d'ATDD.
- Méthodes similaires : elles ont leur propre cycle qui les rend à la fois similaires à TDD, mais structurellement différentes.
  - *Acceptance Test-Driven Development* (ATDD)
  - *Story Test-Driven Development* (STDD)
  - *Test && Commit \|\| Revert* (TCR)

## TDDflow : versionnage avec TDD

TDDflow peut se greffer à n'importe quel modèle des flux de versionnage, tels que GrootFlow, Gitflow ou *Trunk-Based Development*. En plus de TDD, il est compatible avec *Bug-Driven Development*, *Documentation-Driven Development*, et même TCR (*Test && Commit \|\| Revert*).

# Acceptance-Test Driven Development (ATDD)

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

## Définition d'ATDD

ATDD est une méthode incrémentale qui guide les développements par itérations depuis l'heuristique et la capture du besoin jusqu'à aboutir à une solution testée littéralement, voire visuellement, et démontrable, en renforçant la communication et la collaboration, afin de livrer régulièrement un produit toujours plus satisfaisant aux utilisateurs.

## Cycle 4D d'ATDD

Le macro-cycle d'ATDD se déroule en 4 étapes.

![Cycle 4D d'ATDD](ressources/schemas/4d_atdd_cycle__fr.png)

À chaque itération :
1. Discuter
2. Distiller
3. Développer
4. Démontrer

# Behavior-Driven Development (BDD)

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

## Définition de BDD

BDD est une méthode incrémentale qui guide les développements par macro-cycles depuis l'heuristique et la capture du besoin jusqu'à aboutir à une solution auto-spécifiée, auto-documentée et démontrable, en renforçant la communication et la collaboration, afin de livrer continuellement un produit toujours plus satisfaisant aux utilisateurs.

# Foire Aux Questions

## Faut-il se former à TDD dès le début de sa carrière ?

Quand on se forme à un langage de programmation, on écrit généralement des morceaux de code pour réaliser de toutes petites tâches, comme autant d'exercices. On a donc le choix de vérifier le résultat soit en l'affichant en console (test manuel), soit en le testant en utilisant un framework de test (test automatisé). La deuxième option est bien meilleure, car on développe deux compétences conjointement au lieu d'une, car on apprend plus vite en maîtrisant ce qu'on fait, car automatiser ses tests n'est plus un sujet tabou. Ensuite, analyser un problème en sous-problèmes et commencer à définir un sous-problème en le décrivant sous la forme d'un test automatisé, tout cela avant de foncer tête baissée dans la recherche d'une solution, c'est déjà pratiquer TDD.

Au final, viser TDD même en commençant par des petits tests automatisés sur des petits morceaux de code est à mon avis la meilleure façon d'apprendre un langage de programmation, qu'on soit junior ou sénior d'ailleurs. On peut voir fleurir beaucoup de billets ou d'articles pour dissuader les juniors de s'intéresser à TDD dès le début... Plus tôt vous adopterez cette gymnastique de l'esprit, moins vous devrez désapprendre pour réapprendre, plus vite TDD sera une évidence, la vôtre.

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

## Pourquoi TDD n'est-il pas une stratégie de test ?

Que cela signifie-t-il de dire que TDD n'est pas une stratégie de test ?

Passons au crible TDD et stratégie de test pour les comparer et y voir enfin plus clair.

QQOQCCP | TDD | Stratégie de test
:-----: | --- | -----------------
Qui ? | TDD a été imaginé par des développeurs pour des développeurs. | Une stratégie de test est généralement conçue par un QA Manager ou un Test Leader, pour être appliquée par des testeurs et des développeurs.
Quoi ? | TDD est une méthode de développement qui s'appuie sur les tests avant codage afin de décrire un problème de développement à résoudre. | Une stratégie de test est un ensemble de décisions sur la manière de gérer les activités de test.
Où ? | TDD est pratiqué pendant le codage seulement. | Une stratégie de test est à l'œuvre partout où les tests peuvent être mis à profit dans le processus de création d'un produit, depuis l'idéation (*shift-left testing*) jusqu'à l'exploitation (*shift-right testing*).
Quand ? | Les prémisses de TDD remonteraient à 1999. La méthode a évolué depuis. | Une stratégie de test est élaborée spécifiquement pour un produit logiciel, après avoir défini une politique de test. Elle est mise à jour au besoin au cours de la vie du produit.
Comment ? | TDD n'apporte aucune réponse sur les formes de test à employer. Il faut seulement que les tests automatisés avec TDD soient FIRST pour en tirer profit. C'est pourquoi TDD est agnostique de toute forme de test. | Une stratégie de test sélectionne et définit les formes de test à employer pour réduire le nombre et le risque des défaillances en production.
Combien ? | TDD ne prescrit rien quant au nombre de tests à automatiser. | Une stratégie de test doit répartir l'effort de test, pour les tests manuels comme pour les tests automatisés, entre les différentes formes de test sélectionnées pour un produit.
Pourquoi ? | Les praticiens de TDD estiment qu'un grand bénéfice parmi d'autres de TDD est de consacrer beaucoup plus de temps à développer un logiciel qu'à le déboguer pas à pas à chaque changement. | Une stratégie de test permet d'aligner une organisation, c'est-à-dire de coordonner les acteurs impliqués, quant aux moyens à mettre en œuvre pour livrer un produit conforme aux attentes, qu'il s'agisse des attentes des utilisateurs, d'attentes réglementaires, d'attentes contractuelles, etc.

**NB :** L'incompréhension de ce qu'est une stratégie de test est à l'origine d'un point de friction permanent dans la communauté des développeurs, qui essaient d'y remédier en tordant la définition de test unitaire plutôt que de réfléchir à une stratégie de test d'ensemble. Dans une stratégie de test, on doit à un moment sélectionner différentes formes de test pertinentes pour atteindre des objectifs de l'entreprise. TDD va seulement pousser à automatiser une toute petite partie de ces formes de test pour faciliter les développements. Les enjeux ne sont pas du tout les mêmes.

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

## Que signifie unitaire dans le contexte de TDD ?

En vérité, unitaire signifiait **assertion** quand Robert C. Martin l'a utilisé dans ses premières formulations des trois lois de TDD, entre 2005 et [2008][Clean Code/The Three Laws of TDD]. Toutes les confusions et le capharnaüm qui règne dans la communauté du *Software Craftsmanship* trouvent leur origine ici. Comme Robert C. Martin s'est aperçu de sa bévue, sa [dernière formulation][Martin/The Cycles of TDD] en 2014 voit le terme unitaire enfin supprimé. Car unitaire désigne et doit continuer à désigner une **unité de programmation**, de sorte que cette unité de programmation dépend en fait du paradigme de programmation (une classe en programmation orientée objet, une fonction en programmation fonctionnelle, une procédure en programmation procédurale, etc), et non des tests. Quand vous voudrez parler d'un test dont le sujet n'est pas une unité de programmation, vous devrez vous intéresser à la typologie et taxonomie des tests logiciels, afin de recourir au vocable adéquat.

Car rien de tel pour semer le chaos et la discorde que d'employer un même mot pour désigner des choses différentes.

> Mal nommer un objet, c'est ajouter au malheur de ce monde.
-- Albert Camus, Sur une philosophie de l'expression, 1944

M'étant longuement penché sur la typologie des tests, je vous recommande le terme de **test métier** pour désigner un test fonctionnel qui traverse un groupe de classes comme sujet de test et dont l'objectif est de vérifier une règle métier, d'où son nom. Test unitaire et test métier forment le groupe des tests comportementaux, car ils servent tout deux à vérifier des comportements d'un logiciel.

En pratiquant TDD, nous sommes ainsi amenés à réaliser surtout des tests métier, et plus rarement des tests unitaires, selon que nous voulons tester une règle métier complète ou un petit algorithme, le principal étant que les tests soient résilients face au remaniement de code. Bien sûr, cela n'exclut pas de recourir plus souvent à des tests unitaires pour d'autres besoins ou pour d'autres pratiques que TDD. Nous serons alors bien contents de les retrouver, indemnes et fidèles à eux-mêmes.

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

## Fait-on vraiment des tests d'acceptation en TDD, ATDD ou BDD ?

Par définition dans le domaine du test logiciel, un test d'acceptation utilisateur porte sur la **satisfaction d'un besoin de l'utilisateur final**. Un tel test a pour résultat une **appréciation nuancée et subjective**, formulée au moins oralement, sinon par écrit, à propos de l'adéquation du produit au besoin. Les seules personnes capables de faire des tests d'acceptation utilisateur sont donc les utilisateurs finaux eux-mêmes.

Quand on automatise un test quelconque, l'automate de test ne peut fournir qu'un résultat binaire de succès ou d'échec, qui sanctionne la conformité non pas à un besoin mais à une spécification. Du fait de cette différence fondamentale entre tests d'acceptation utilisateur et tests automatisés, aucun des tests automatisés avec le concours des méthodes *DD ne saurait être un test d'acceptation utilisateur, jamais, par essence.

Si les tests de BDD sont appelés des tests d'acceptation dans la littérature, c'est par abus de langage : même si les tests de BDD émanent à l'origine de la voix des utilisateurs, ils cessent d'être des tests d'acceptation utilisateur à proprement parler dès lors qu'ils sont gérés par des développeurs ou des testeurs, qu'ils soient automatisés ou exécutés manuellement.

Autant il est possible de s'approprier et de détourner un test d'acceptation utilisateur en tant que développeur ou testeur afin de l'automatiser, autant le test automatisé ainsi obtenu n'est plus un test d'acceptation utilisateur. A fortiori, un test unitaire ne peut pas être un test d'acceptation utilisateur, et un test d'acceptation utilisateur ne peut pas être unitaire.

QQOQCCP | Test *DD | Test d'Acceptation Utilisateur
------- | --------------- | ------------------------------
Qui ? Réalisé par... | un développeur ou testeur | un utilisateur final
Quoi ? Le résultat est... | un succès ou un échec | une appréciation nuancée et subjective
Où ? Exécuté dans un environnement de... | test | production
Quand ? Exécuté... | pendant les développements | après livraison
Comment ? | Automatisé ou manuel | Manuel seulement
Combien ? | Très nombreux | Peu nombreux
Pourquoi ? Pour... | vérifier la conformité à une spécification | valider la satisfaction d'un besoin

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

## TDD permet-il vraiment d'en finir avec le débogage ?

Le débogage relève du test dynamique et manuel après codage, où un développeur vérifie l'état interne du logiciel en contrôlant les valeurs des variables, ainsi que le chemin d'exécution. Comme il peut y avoir une distance importante en nombre de lignes de code entre le début de l'exécution et les composants à déboguer, un développeur utilise des points d'arrêt, puis procède en pas à pas. En général, on fait appel au débogage, non pas pour vérifier qu'un logiciel fonctionne, mais pour trouver la cause racine d'un défaut déjà identifé, et le placement des points d'arrêt se précise progressivement. Cela signifie au moins trois choses importantes.
1. Lors d'un test par débogage, il y a des composants sur lesquels se focaliser, et d'autres au contraire à ignorer.
2. Le débogage est assimilable à un test en boîte blanche, voire à une suite de tests en boîte blanche, pratiqués après qu'un autre test plus grosse maille, probablement en boîte noire, fut en échec.
3. Le débogage est utilisé après qu'un certain laps de temps s'est écoulé depuis l'introduction d'un défaut.

Les trois points précédents entraînent respectivement trois conséquences.
1. Plus le code est complexe dans les composants ciblés et plus les composants ciblés sont nombreux, plus la charge mentale du développeur est élevée, plus sa tâche est difficile.
2. Le débogage fait partie d'une activité de test qui s'inscrit déjà à plusieurs niveaux de test. Par exemple, on teste fonctionnellement une interface utilisateur ou une API, avant d'en arriver à déboguer des composants de type classe ou fonction, depuis les couches supérieures vers les couches inférieures de l'architecture. Dans cette approche du test, les tests les plus représentés dans le processus de développement sont donc des tests de haut niveau (en s'éloignant du code), et les tests les moins représentés ceux de bas niveau (au plus près du code) : cette approche du test favorise les tests les plus coûteux à réaliser, qui sont aussi ceux qui ne permettent pas de localiser la source précise d'un défaut.
3. Le coût d'une correction par débogage n'est jamais anodin, et il augmente rapidement en fonction du délai entre l'introduction d'un défaut et sa correction. Ce coût de correction pèse de façon significative sur la capacité à développer des fonctionnalités à valeur ajoutée.

Quelles leçons pouvons-nous en tirer ?
1. La correction d'un défaut sera d'autant plus aisée que la charge mentale du développeur est réduite, autrement dit que le code est simple à l'intérieur des composants et que les responsabilités des composants sont bien découpées. Or on peut dire exactement la même chose au sujet d'un test automatisé : l'automatisation d'un test sera d'autant plus aisée que le code est simple à l'intérieur des composants et que les responsabilités des composants sont bien découpées. Si le test est automatisé avant codage, il faudra réaliser un développement en fonction du test, en appliquant les principes de simplicité, de cohésion et de découplage. Pourquoi ne pas faire d'une pierre deux coups, en automatisant les tests avant codage pour améliorer la conception logicielle et en utilisant ces mêmes tests pour localiser la source d'un défaut ?
2. Plus un test est de bas niveau, plus il contribue à localiser aisément la source précise d'un défaut, et ce à moindre coût. Cela ne veut pas dire que les tests de plus haut niveau sont inutiles : ils sont simplement complémentaires en testant un logiciel de façon différente, pour détecter d'autres types de défauts. Ainsi pourquoi ne pas développer un logiciel en favorisant les tests de bas niveau et où les tests de haut niveau en moindre nombre viennent compléter les premiers ? On optimise ainsi le bénéfice des tests automatisés par rapport à leur coût.
3. En automatisant les tests de concert avec le développement, un développeur se donne les moyens de détecter un défaut au moment même où il a été introduit. Ainsi, le développeur corrige ce défaut quand il coûte le moins cher à corriger. Il économise même le coût du changement de contexte en restant concentré sur son objectif présent.

En résumé, une telle approche de développement consisterait à coder après avoir automatisé un test pour tirer la conception d'un logiciel vers plus de simplicité, à localiser la source précise des défauts en s'appuyant sur des tests les moins coûteux à automatiser et les plus rapides à exécuter, à corriger les défauts le plus tôt possible en exécutant les tests en continu. Non seulement cette approche est plus efficace, mais ce faisant, nous n'aurions plus besoin de déboguer le code ligne après ligne, variable après variable, embranchement après embranchement. Je vous laisse deviner : cette méthode existe déjà, c'est TDD.

![Drive change for Spec + Test + Code with Chrysocode](assets/images/bannière_stardd.png)

# Références bibliographiques

- Robert C. Martin, Clean Code, A Handbook of Agile Software Craftsmanship, 2008, p. 122
- [Robert C. Martin (Uncle Bob), The Cycles of TDD, 2014](http://blog.cleancoder.com/uncle-bob/2014/12/17/TheCyclesOfTDD.html)
- [TDD Manifesto, Values of TDD](https://tddmanifesto.com/)

[Clean Code/The Three Laws of TDD]: https://amzn.eu/d/65hsB4L "Robert C. Martin, Clean Code, A Handbook of Agile Software Craftsmanship, 2008, p. 122"

[Martin/The Cycles of TDD]: http://blog.cleancoder.com/uncle-bob/2014/12/17/TheCyclesOfTDD.html "Robert C. Martin (Uncle Bob), The Cycles of TDD, 2014"

[TDD Manifesto/Values]: https://tddmanifesto.com/ "TDD Manifesto, Values of TDD"
