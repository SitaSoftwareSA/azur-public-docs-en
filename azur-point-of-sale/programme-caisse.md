# Programme Caisse

### Lancement du programme

Le programme Azur P.O.S. se lance automatiquement au démarrage de la caisse.

Le programme vous demande alors de vous identifier en tant qu’utilisateur caisse.\
Ceci se fait dans la fenêtre « Log In ».

![](<../.gitbook/assets/image (24).png>)

Dans le cas où un mot de passe a été défini pour l’utilisateur, cette fenêtre apparait.

![](<../.gitbook/assets/image (81).png>)

Il suffit donc d’entrer le mot de passe correspondant à l’utilisateur choisi pour accéder au programme.

Attention : le programme fait la différence entre les minuscules et les majuscules.\
Par défaut les caractères sont en majuscule, le bouton « Minuscules » permet de les mettre en minuscule.

Une fois le mot de passe saisi, un clic sur le bouton « Valider » permet d’accéder à azur PoS.

{% hint style="info" %}
Le programme apparaît dans la langue de l’utilisateur.

Il est possible pour l’utilisateur de s’identifier avec une carte à code-barres, magnétique, badge magnétique ou clé Dallas.
{% endhint %}

![](<../.gitbook/assets/image (32).png>)

### Description de la fenêtre principale

Après avoir choisi son utilisateur, cette fenêtre apparaît :

•           En haut de l’écran se trouve la barre « poids/prix », uniquement si la caisse est une balance poids/prix.

•           En dessous de la barre « poids/prix » se trouve la barre « info ».

•           Au centre à droite de l’écran se trouvent la barre « famille d’articles » et la «page des articles» correspondants.

•           Au centre à gauche de l’écran se trouvent toutes les informations concernant l’encaissement en cours : les articles déjà sélectionnés dans la zone « Ticket en cours» et l’article choisi dans la zone « Article en cours » ainsi que le total du ticket.

•     En bas de l’écran se trouve la Barre des utilisateurs.

![](<../.gitbook/assets/image (385).png>)

#### Barre poids/prix

![](<../.gitbook/assets/image (361).png>)

Ces trois informations sont affichées également sur le display client et seront aussi imprimées sur le ticket de caisse.

#### Barre d’information

Sur la barre « info » vous trouverez :

•           A  droite le nom de l’utilisateur actuellement en cours ainsi que l’heure.

•           A gauche, vous pouvez voir aussi le nom du client, si une carte client a été scannée (uniquement avec l’option Azur Fidelity)

•           Au centre, un message d’information peut apparaître par exemple quand il faut introduire une quantité pour un article de type « unité ».

![](<../.gitbook/assets/image (378).png>)

#### Famille d’articles

Avec les flèches, vous pouvez naviguer entre les différentes familles d’articles.

En appuyant sur une case, la page d’articles change automatiquement.

![](<../.gitbook/assets/image (379).png>)

La page « home » permet d’avoir des boutons comme raccourcis sure les pages articles.

![](<../.gitbook/assets/image (396).png>)

#### Page des articles

En sélectionnant un article, la zone « Article en cours » se met automatiquement à jour.

\-      S’il s’agit d’un article de type « unité » (un article à la pièce par exemple), la zone article en cours renseigne l’utilisateur : la quantité est par défaut à 1 et on peut enregistrer une quantité différente avec le pavé numérique.

\-      La case « % » permet à l’utilisateur d’attribuer une réduction en pourcentage sur l’article sélectionné.

\-      S’il s’agit d’un article de type « poids », la relation avec la balance est automatique et le poids s’affiche immédiatement.

![](<../.gitbook/assets/image (413).png>)

#### Barre des utilisateurs

![](<../.gitbook/assets/image (384).png>)

En appuyant sur l’utilisateur, l’article sélectionné sera validé et ajouté sur le ticket en cours de l’utilisateur choisi.

Si aucun article n’a été sélectionné, les données du ticket seront rafraîchies.

Le bouton « autre opérat. » permet d’ajouter un autre utilisateur à la barre des utilisateurs.

Dans le cadre d’une connexion à une balance poids/prix :

·         Le bouton « Mise à zéro » permet de remettre la balance à zéro, lorsque celle-ci n’affiche pas exactement 0,000.

·         Le bouton « Tare » permet de déduire la masse d’un objet (une boîte par exemple) avant de commencer à peser l’article sélectionné.

&#x20;

Le bouton « Fermer » permet de fermer un utilisateur. Il sera donc enlevé de la barre des utilisateurs.

Le bouton « Verrouillage » permet de verrouiller l’écran de la balance lorsque l’on veut nettoyer l’écran par exemple.

Pour déverrouiller, il suffit d’appuyer sur l’écran. Un mot de passe est alors demandé. Par défaut ce mot de passe est « azur » en minuscule, mais il peut être changé.

&#x20;

Le bouton « Reimp. Ticket » permet de réimprimer un ticket de caisse.\
Une fenêtre s’ouvre permettant la réimpression d’un ticket.\
Par défaut, le numéro du dernier ticket de caisse qui a été imprimé est affiché à l’écran.\
Pour choisir un autre ticket, il suffit d’appuyer sur le bouton « Changer » et d’entrer le numéro du ticket que l’on veut imprimer.\
Ensuite, il suffit d’appuyer sur le bouton « Imprimer » pour réimprimer le ticket de caisse dont le numéro est affiché à l’écran.

![](<../.gitbook/assets/image (352).png>)

Le bouton « Voir tickets en attente » permet de voir et reprendre un ticket mis en attente au préalable.

![](<../.gitbook/assets/image (427).png>)

#### Ticket et article en cours

![](<../.gitbook/assets/image (355).png>)

#### Choix de l’article

![](<../.gitbook/assets/image (431).png>)

### Suppression d’un article ou d’un ticket

#### Suppression d’un article

![](<../.gitbook/assets/image (444).png>)

Sélectionnez l’article à supprimer. Il sera marqué avec une ligne bleue.\
Cliquez sur le bouton « SUPP » pour supprimer cet article du ticket de caisse.

Par défaut, l’article n’apparaît pas dans les lignes du ticket de caisse (il est possible de configurer son impression avec ajout d’une quantité en négatif)

Voici le résultat après la suppression de l’article sélectionné ci-dessus.

![](<../.gitbook/assets/image (411).png>)

#### Annulation d’un ticket

Cliquez sur le bouton « Options »  en bas à droite de l’écran, cliquez ensuite sur le bouton « Annuler ticket en cours ».\
\
Une fenêtre d’avertissement apparaît alors à l’écran vous demandant de confirmer la suppression du ticket en cours.

![](<../.gitbook/assets/image (440).png>)

Pour confirmer la suppression, appuyer sur le bouton « Oui ».\
Tous les articles du ticket de caisse vont être supprimés, le ticket sera donc mis à zéro.\
Il sera ensuite clôturé et ne sera pas imprimé.

L’annulation d’un ticket peut être possible uniquement pour le responsable du magasin, ou pour certains opérateurs de caisse.

### Clôture d’un ticket

Appuyez sur le bouton « Ticket » à gauche de la barre des utilisateurs

![](<../.gitbook/assets/image (437).png>)

Les informations de clôture du ticket apparaissent:

![](<../.gitbook/assets/image (436).png>)

La case « Remise % » permet de faire une remise (en pourcentage) sur le montant total du ticket.

&#x20;

Le montant payé est par défaut le montant total du ticket.

Vous avez la possibilité d’encoder un autre montant payé, s’il s’agit d’un paiement en espèces.

&#x20;Les boutons « CPT, VIS, BAN, EUR, MAE, MAS, PRO » représentent les abréviations des modes de paiement disponibles. Vous pouvez sélectionner un maximum de 12 modes de paiement avec également des automates de paiement en espèces.\
&#x20;

Les boutons « DE, FR, NL, GB » sont les différentes langues possibles pour le ticket de caisse.

Une langue choisie lors de la configuration d’Azur PoS est toujours sélectionnée par défaut mais vous pouvez la changer suivant la langue parlée avec le client (surtout dans les zones touristiques par exemple).

&#x20;Le bouton « OK » permet de valider les opérations de paiement de cette dernière fenêtre.

Le bouton « Correction Ticket » permet de revenir à l’écran précédent et permet donc à l’utilisateur de modifier le ticket.

#### Pour clôturer le ticket

Paiement en espèces

Entrer le montant donné par le client dans la zone « Montant payé » et valider ensuite le mode de paiement avec le bouton « OK ».

![](<../.gitbook/assets/image (390).png>)

Ci-dessus, le client a donné 15 euros.\
La case « A rendre » contient le montant que l’utilisateur doit rendre au client.

S’il y a une connexion d’Azur PoS à un automate de paiement, les sommes enregistrées et à rendre sont gérées par la machine.\
Ensuite, il suffit d’appuyer sur le bouton « OK + Impression » pour clôturer le ticket de caisse et l’imprimer.\
Le tiroir-caisse est configuré pour s’ouvrir automatiquement à l’impression du ticket.

Paiement par carte

Il suffit de choisir le mode de paiement et ensuite de valider avec le bouton « OK ».\
Le montant ne peut pas être changé lorsque c’est un paiement par carte, le programme prend automatiquement le montant total.

Il suffit ensuite d’appuyer sur le bouton « OK + Impression » pour clôturer le ticket de caisse et l’imprimer.

{% hint style="info" %}
_Remarque :_\
&#xNAN;_&#x50;lusieurs modes de paiement peuvent être combinés et le montant restant à payer est automatiquement recalculé. Dans ce cas, le paiement en espèces doit toujours anticiper le paiement par cartes de crédit._
{% endhint %}

#### Impression d'étiquettes

![](<../.gitbook/assets/image (425).png>)

Le bouton « Etiquette » permet d'imprimer une étiquette. On sélectionne d’abord un article on pose la quantité désirée sur la balance et une fois que le poids est stable, on appuie sur le bouton « Etiquette ».

Il ne vous reste à présent plus qu'à coller l'étiquette imprimée sur l’article que vous avez pesé. Ainsi les clients pourront choisir des articles préparés à l'avance et il suffira de scanner le barre-code sur l'étiquette.

#### Ouverture du tiroir-caisse

![](<../.gitbook/assets/image (412).png>)

Le bouton « Tiroir » permet d’ouvrir le tiroir-caisse indépendamment d’une clôture de ticket.

Un mot de passe peut être défini pour ce bouton ou un droit donné à un ou plusieurs utilisateurs.

#### Carte de fidélité

![](<../.gitbook/assets/image (353).png>)

### Les remises

#### Remise sur une ligne

Quand un article est sélectionné on à la possibilité d’introduire une remise par ligne, exprimée en pourcentage.

![](<../.gitbook/assets/image (399).png>)

Quand on se positionne sur le champ de remise on doit composer le mot de passe défini à l’avance, pour que le champ soit accessible.

![](<../.gitbook/assets/image (362).png>)

#### Remise globale

![](<../.gitbook/assets/image (393).png>)

Quand on se positionne sur le champ de remise globale (comme pour le champ de remise par ligne) il est possible d’encoder un mot de passe défini à l’avance, pour que le champ soit accessible:

![](<../.gitbook/assets/image (392).png>)

### Les « Options »

![](<../.gitbook/assets/image (377).png>)

#### Imprimantes

![](<../.gitbook/assets/image (426).png>)

Lorsque vous cliquez dessus, une fenêtre de configuration apparaît et vous pouvez alors choisir ou modifier les imprimantes que vous voulez utiliser.

![](<../.gitbook/assets/image (416).png>)

#### Reprise ticket

![](<../.gitbook/assets/image (358).png>)

Il suffit de cliquer sur le bouton « Reprise ticket ». Une fenêtre apparaît ensuite demandant un mot de passe. Par défaut le mot de passe est « azur » en minuscule.

![](<../.gitbook/assets/image (407).png>)

Après avoir entré le mot de passe et cliqué sur le bouton « Valider », une deuxième fenêtre apparaît vous demandant le numéro du ticket à reprendre. Lorsque vous avez saisi le numéro du ticket, cliquez sur le bouton « Valider ». Le ticket sélectionné apparaît donc à l’écran et il est alors possible de le modifier.

![](<../.gitbook/assets/image (370).png>)

#### Rapport de caisse

![](<../.gitbook/assets/image (415).png>)

Voici comment se présente la fenêtre du rapport de caisse :

A gauche, sont affichées les ventes effectuées pendant la journée ainsi que le nouveau fond de caisse théorique.

A droite, les différentes cases vous permettent d’indiquer le nombre de pièces et de billets que vous avez dans votre tiroir-caisse (A remplir uniquement lorsque vous faites le rapport de caisse définitif).

![](<../.gitbook/assets/image (394).png>)

#### Rapport de caisse provisoire (de type x)

Lorsque vous choisissez de faire un rapport de caisse provisoire, il vous suffit de ne pas cocher « Faire rapport de caisse définitif » et d’appuyer sur le bouton « Valider » Le rapport de caisse provisoire s’imprime directement à l’imprimante. Vous pouvez faire autant de rapport provisoire que vous voulez sur la journée.

#### Rapport de caisse définitif (de type z) (un seul par jour)

Lorsque vous choisissez de faire un rapport de caisse définitif, il vous suffit de cocher « Faire rapport de caisse définitif » et vous devez remplir le nombre de pièces et de billets que vous avez en caisse.

![](<../.gitbook/assets/image (373).png>)

### Consultation des rapports de caisse définitifs précédents

![](<../.gitbook/assets/image (360).png>)

![](<../.gitbook/assets/image (382).png>)

### Option : Commande client

La commande du client est prise soit au magasin soit par téléphone.

Cette option permet de voir à quelle étape la commande se trouve en production (pas encore traitée, en cours, prête).

Quand c’est un article au poids, il est possible de noter le poids désiré.

A la préparation de la commande, il faudra peser l’article pour modifier le ticket avec le poids précis et donc le montant recalculé.

Un acompte peut être pris à la commande et apparaît sur le ticket. A l’enlèvement de la commande apparaît le montant de l’acompte déjà payé.

Si on n’est pas intéressé par le suivi des commandes avec l’option acompte, on peut encaisser quand-même un montant donné en acompte.

### Les opérations de caisse

![](<../.gitbook/assets/image (388).png>)

Lorsque vous cliquez sur ce bouton, la fenêtre ci-dessous apparaît:

![](<../.gitbook/assets/image (438).png>)

#### Les dépenses

Pour enregistrer une dépense dans la caisse, vous sélectionnez le bouton « Dépenses ». Vous indiquez le montant de la dépense dans la case « Dépenses ». La case « Description » vous permet d’indiquer la raison de la dépense ou le n°de la pièce comptable. Cette case doit obligatoirement être remplie pour pouvoir valider la dépense. Lorsque les 2 cases sont remplies, vous pouvez enregistrer la dépense avec le bouton « Valider ».

![](<../.gitbook/assets/image (402).png>)

#### Les versements

Pour enregistrer un versement dans la caisse, vous sélectionnez le bouton « Versements ». Vous indiquez le montant du versement dans la case « Versements ». La case « Description » vous permet d’indiquer la raison du versement. Cette case doit obligatoirement être remplie pour pouvoir valider le versement. Lorsque les 2 cases sont remplies, vous pouvez enregistrer le versement avec le bouton « Valider ».

#### Le fond de caisse

Pour enregistrer un fond de caisse, vous devez sélectionner le bouton « Fond caisse ». Vous indiquez le montant dans la case « Fond de caisse » et vous enregistrez le fond de caisse saisi avec le bouton « Valider ».

![](<../.gitbook/assets/image (408).png>)

### Mode Caisse et mode Balance

Dans le cas où votre entreprise serait dotée d’une balance avec tiroir-caisse intégré, il vous est possible d’utiliser une nouvelle fonction d’Azur POS : Le changement de mode.

Dans certains cas, il est utile de pouvoir utiliser une caisse juste en tant que balance ; par exemple pour préparer une corbeille d’articles qui ne sera qu’encodée quelques jours plus tard et vice-versa.

Pour ces cas de figure, Azur POS propose la fonction de changement de mode, avec laquelle il est très simple de transformer sa caisse en balance et inversement.

#### Changement de mode

Celui-ci s’effectue à partir de la barre inférieure gauche, là où se trouve en temps normal le bouton « Etiquette ».

![](<../.gitbook/assets/image (374).png>)

Après avoir appuyé sur ce bouton, une nouvelle fenêtre s’affiche indiquant les différents modes disponibles:

![](<../.gitbook/assets/image (381).png>)

Choisissez le mode correspondant et confirmez ensuite avec le bouton OK en bas de la fenêtre.

#### Mode Caisse

Le mode caisse est la version standard d’Azur POS.

#### Mode Balance

Le mode balance peut utiliser toutes les fonctions d’Azur POS, à la différence près que sous le mode balance, rien n’est définitivement encodé dans les achats.

A savoir : tout ticket créé sous ce mode n’est "que provisoire" et n’a aucune valeur représentative, ce n’est qu’après avoir ré-encodé le ticket sous le mode caisse que celui-ci est vraiment enregistré dans Azur POS.

Le ticket ainsi créé est logiquement exempt de la TVA, du mode de paiement, du montant rendu et de la devise utilisée. Ceux-ci font place à un code-barre qui peut être scanné dans le mode caisse afin de créer le ticket définitif.

#### Communication entre balances et caisses

Comme énoncé plus haut, tout ticket créé sous le mode balance doit être encodé (ou supprimé) postérieurement. Il n'est pourtant pas toujours possible de changer une balance qui est utilisée en permanence. C'est pourquoi Azur POS communique automatiquement d'une balance ou caisse à l'autre.

Pour encoder le ticket déjà créé dans le mode balance,  il suffit de scanner le code-barre avec Azur POS en mode caisse ou en encodant le numéro de ticket manuellement.

{% hint style="info" %}
Remarques:

\-      Votre balance/caisse s’ouvre par défaut, en tant que caisse ou en tant que balance, suivant vos besoins.

\-      Il n’est pas possible de changer de mode si un ticket est en cours. Il faut soit encoder ce dernier, soit le supprimer avant de pouvoir changer de mode.

\-      Surtout, n'oubliez pas de reprendre tout ticket créé sous le mode balance dans le mode caisse. Les tickets non repris ne seront pas affichés dans le journal de ventes.
{% endhint %}
