# Facturation

### Release Notes

Version 2.1 (23.04.2020)

Dans la sélection des documents pour remise, ajout d’un champ «calcul remise »

* Une fois le document sélectionné pour remise (F6), le champ calcul remise est automatiquement coché.
* L’utilisateur peut le décocher avec le bouton prévu à cet effet ou la touche F7.
* Cette option permet d’inclure un document dans une remise mais forcer de ne pas calculer de remise.

Version 2.0 (20.04.2020)

* Dans l’historique, affiche à l’utilisateur la liste des documents d’un client dans une remise.
* Ajoute la possibilité d’enlever un document d’une remise.
* Ajoute la possibilité d’ajouter un document dans une remise.
* Ajoute la possibilité d’imprimer une sélection de job pour une remise.
* Le fichier txt s’exporte suivant la configuration de l’écran.

### Remises clients

Ce module a pour objectif de générer des remises comme des commissions à certains clients.

Le module se décompose en 4 grandes étapes



Sélection des documents

Validation des documents

Historique / Résultat

Configuration des remises

#### Sélection des documents

Ci-dessous l’écran de sélection des documents. Dans cette étape l’utilisateur va pouvoir sélectionner les documents qui seront repris dans le calcul des remises.

Critères de recherche

![](<../.gitbook/assets/image (429).png>)

Critères de sélections standard

![](<../.gitbook/assets/image (401).png>)

Critères spécifiques

![](<../.gitbook/assets/image (406).png>)

* **Client même adresse**, affiche les clients qui sont facturés et livrés à a même adresse. Le client est le même
* **Document soldé** permet d’afficher les documents payés.
* **Client actif remise** permet d’afficher les clients pour lesquelles vous avez spécifier un code remise

```
Client.Code_remise 
 0 -> Aucune remise accordée
>0 -> Remise accordée
```

* **Document soldé avant X jours**, permet de filtrer les clients qui soldent les factures rapidement

Nombre de jour de contrôle de paiement

![](<../.gitbook/assets/image (433).png>)

1. C’est le nombre de jour X qui permettra au programme de d’afficher si oui ou non, le client a payé sa facture dans un délais de X jours.
2. Ce paramètre est à définir dans les options de l’écran.
3. Bouton options en haut à droite de l’écran ![alt](https://docs.sitasoftware.lu/erp/fr/images/bouton_option.fr.png)

#### **Recherche**

Cliquez sur le bouton recherche.

Ci-dessous un résultat de recherche et la description des champs du grid

![](<../.gitbook/assets/image (447).png>)

![](<../.gitbook/assets/image (445).png>)

#### **Actions**

Descrip**t**ion des différentes actions possibles à l’étape 1

![](<../.gitbook/assets/image (430).png>)

**PAIEMENT OK / ANNULER**

Pour le document actif ou pour une sélection de document

* Permet à l’utilisateur d’accorder une remise malgré le fait que le client n’a pas payé la facture dans les X jours
* Permet à l’utilisateur d’annuler l’accord de remise

**OK REMISE / ANNULER**

Pour le document actif ou pour une sélection de document

* Permet à l’utilisateur de placer la/les facture(s) dans la prochaine remise
* Permet à l’utilisateur d’enlever la/les facture(s) de la prochaine remise

**AJOUTER DANS UNE REMISE**

Permet d’ajouter un document dans une remise existante

**REPORT GLOBAL**

Permet d’afficher à l’écran un rapport global provisoire avec le résumé de la remise

**REPORT CLIENTS**

Permet d’afficher un rapport détaillé pour tous les clients qui seront dans la prochaine remise

**REPORT CLIENT**

Permet d’afficher un rapport détaillé pour le client actif

**HISTORIQUE**

Permet de naviguer vers l’étape 3 du module

**DATE TRAITEMENT**

Est la date qui est utilisée pour les calculs provisoires

**CONTRÔLE POUR REMISE**

Permet de naviguer vers l’étape 2 du module

#### Validation des documents <a href="#validation-des-documents" id="validation-des-documents"></a>

À cette étape, l’utilisateur peut voir et ainsi vérifier la liste des clients/factures qui seront dans la prochaine remise

![](<../.gitbook/assets/image (420).png>)



Pour créer la remise cliquer sur le bouton ![](<../.gitbook/assets/image (387).png>)

Une fois le traitement encours, vous pouvez visualiser ce que le programme est en train d'exécuter.

![](<../.gitbook/assets/image (389).png>)

Pour revoir les derniers **logs** cliquez sur le bouton ![alt](https://docs.sitasoftware.lu/erp/fr/images/bouton_log.fr.png) situé en haut à droite de l’écran.

![](<../.gitbook/assets/image (262).png>)

Une fois le traitement effectué, vous pouvez choisir de créer ou non les jobs. Si vous répondez non, vous pourrez le faire lors de l’étape 3. Le programme vous ouvre automatiquement dans la partie historique une fois que tout est fini.

#### Historique <a href="#historique_1" id="historique_1"></a>

La recherche vous permet d’afficher la liste des remises entre deux dates.

![](<../.gitbook/assets/image (182).png>)

Dans la grille de gauche vous visualisez la liste des remises et dans la grille de droite la liste des clients avec la remise.

![](<../.gitbook/assets/image (231).png>)

#### Actions <a href="#actions_1" id="actions_1"></a>

![](<../.gitbook/assets/image (252).png>)

**GÉNÉRER JOBS**

Permet de générer les jobs si cela n’a pas été fait à l’étape 2

**JOB GLOBAL**

Permet de visualiser le job global qui sera défini

**JOB CLIENT**

Permet de visualiser le job du client dans le DMS

**GÉNÉRER FICHIER**

Permet d’exporter un fichier avec le détail de la remise par client. L’emplacement se défini via le bouton option en haut à droite

**ENLEVER LE DOCUMENT DE LA REMISE**

Permet d’enlever le document choisi de la remise. Le job global et le job du client seront à regénérer

**IMPRESSION SÉLECTION**

Choisissez une de vos imprimantes sur laquelle vous voulez imprimer, sélectionner les clients voulu (CTRL+Click) et cliquer sur imprimer

#### Configuration des remises <a href="#configuration-des-remises" id="configuration-des-remises"></a>

Pour configurer les remises cliquer sur le bouton options ![alt](https://docs.sitasoftware.lu/erp/fr/images/bouton_option.fr.png) en haut à droite de l’écran

Ensuite dans l’écran des options, cliquer sur le bouton des **Règles remises**

![](<../.gitbook/assets/image (210).png>)

L’écran de Règles pour les remises s'ouvre. Des règles standards sont déjà encodées

![](<../.gitbook/assets/image (176).png>)

Description des champs de la grille des règles remises

![](<../.gitbook/assets/image (273).png>)

#### Pour activer les remises pour un client <a href="#pour-activer-les-remises-pour-un-client" id="pour-activer-les-remises-pour-un-client"></a>

* Se rendre dans le 321, onlet 5. Relations commericiales, rubrique Remise

![](<../.gitbook/assets/image (249).png>)

{% hint style="info" %}
Il se peut que ce soit un peut différent chez vous.
{% endhint %}

#### Comment faire si je dois changer mes conditions et/ou la remise à partir d’une certaine date ? <a href="#comment-faire-si-je-dois-changer-mes-conditions-etou-la-remise-a-partir-dune-certaine-date" id="comment-faire-si-je-dois-changer-mes-conditions-etou-la-remise-a-partir-dune-certaine-date"></a>

* Se rendre dans l’écran de règle des remises
* Identifier le type de remise qui change
* Cloturer l’ensemble des données de la remise identifiée en mettant une date de fin
* Cloner ces données en mettant la date début voulue et en laissant une date de fin vide
* Enfin changer la remise et/ou les conditions

**Si vous ne mettez pas de date de fin**, et que vous changez simplement de montant de la remise **il ne sera plus possible d’afficher / calculer les chiffre rétroactivement !**

#### Comment faire si j’ai un nouveau client et qu’il va avoir droit à la remise standard ? <a href="#comment-faire-si-jai-un-nouveau-client-et-quil-va-avoir-droit-a-la-remise-standard" id="comment-faire-si-jai-un-nouveau-client-et-quil-va-avoir-droit-a-la-remise-standard"></a>

* Vous ne devez rien faire, comme les remises sont configurées sur le client -1 (tous), il sera automatiquement concerné

#### Comment faire si je décide de donner une remise unique à un client ? <a href="#comment-faire-si-je-decide-de-donner-une-remise-unique-a-un-client" id="comment-faire-si-je-decide-de-donner-une-remise-unique-a-un-client"></a>

* Se rendre dans l’écran de règle des remises
* Identifier le type de remise unique par défaut il s’agit du type 4
* Vérifier qu’il n’a pas encore de données pour ce client
  * Vous pouvez utiliser la grille et faire la recherche sur le n° du client
* Cliquer sur le bouton **Ajouter**

Le programme vous prérempli déjà une partie des champs à saisir

![](<../.gitbook/assets/image (261).png>)

Saisi&#x72;**:**

* Montant du
* Montant au
* N° de client
* Une description
* Et le pourcentage de la remise
* Enfin cliquer sur valider

![](<../.gitbook/assets/image (212).png>)
