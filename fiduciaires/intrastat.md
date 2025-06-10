# Intrastat





Ce chapitre a pour but l'introduction au module "Intrastat" d'**azur**. Ce module vous permet d'automatiser au maximum le remplissage des formulaires pour l'Intrastat. Nous commencerons par le paramétrage correct du dossier, puis on traitera les informations supplémentaires à encoder dans les tables des clients, fournisseurs et articles et finalement sera expliqué l'écran d'encodage Intrastat lui‐même.

![](<../.gitbook/assets/image (121).png>)

### Changement 2021 <a href="#changement-2021" id="changement-2021"></a>

{% hint style="info" %}
info

Dans la mesure où il le numéro de Tva du partenaire (numéro d’identification Intracommunautaire) doit être ajouté au fichier des expéditions des déclarations Intrastat, nous avons décidé d’ajouter un contrôle sur ces numéros afin de garantir que les fichiers soient de qualité. Cela servira également pour les déclarations Etats récapitulatifs de biens et de Services. [plus d'info](https://docs.sitasoftware.lu/fiduciaires/fr/intrastat.fr/#controle-iblc)

Les mêmes contrôles ont été ajoutés dans les Etat récapitulatifs [plus d'info](https://docs.sitasoftware.lu/fiduciaires/fr/intrastat.fr/#module-etat-recapitulatifs)
{% endhint %}

### Le paramétrage du dossier <a href="#le-parametrage-du-dossier" id="le-parametrage-du-dossier"></a>

![](<../.gitbook/assets/image (145).png>)

Après avoir lancé le programme **31. Paramètres du dossier**, vous trouverez sur la 4e page d'onglet les paramètres du module Intrastat. Quoique vous puissiez paramétrer indépendamment l'achat et la vente, ce manuel se limitera à décrire les paramètres pour la vente, puisque le même paramétrage s'applique aussi aux documents d'achat Mode d'encodage: Vous devez choisir le moment auquel vous désirez effectuer l'encodage des données Intrastat. Pendant l'encodage: L'écran d'encodage Intrastat s'ouvre après chaque ligne encodée dans un document de vente/achat. À la fin de l'encodage: L'écran d'encodage Intrastat s'ouvre après avoir validé un document de vente/achat. Externe à l'encodage (option par défaut): **azur** gère une liste des documents qui n'ont pas encore été encodés dans Intrastat. En lançant l'écran 18 Intrastat vous pouvez consulter cette liste et démarrer l'encodage pour les documents désirés. _Voir plus loin dans ce chapitre la partie: encodage Intrastat), http://www.statistiques.public.lu/fr/enquetes/espace-entreprises/intrastat/index.html?highlight=intrastat_

Niveau de seuil: cet encadré contient une liste de tous les mois qui sont contenus dans la période fiscale actuelle. Pour chaque mois (période Intrastat) vous pouvez indiquer le type de la déclaration Intrastat. Vous pouvez choisir (en accord avec vos obligations légales) entre les **types simplifiée, détaillée et dispensée** pour la déclaration.

![](<../.gitbook/assets/image (120).png>)

Pour changer le type de la déclaration d'une période Intrastat, double‐cliquez sur la ligne de cette période dans le tableau.

![](<../.gitbook/assets/image (77).png>)

Il ne vous reste plus qu'à choisir le type selon le chiffre d'affaires de votre entreprise et de cliquer sur le bouton valider. _Assurez‐vous d'avoir bien choisi le type de la déclaration avant de commencer avec l'encodage des données Intrastat pour un mois donné. Une fois que vous aurez saisi des données Intrastat pour un mois, vous ne pourrez plus changer le type de la déclaration pour ce mois‐ci._

Données par défaut: les données que vous entrez ici seront reprises pour les propositions de remplissage des formulaires Intrastat. Il est conseillé de n'entrer ici que les données qui sont valables pour la majorité de vos transactions avec les clients du type 1 (Intracommunautaire). Si par exemple toutes vos marchandises sont transportées par route à l'intérieur du pays vous pouvez indiquer ceci dans cet écran.

![](<../.gitbook/assets/image (89).png>)

Pour ces champs, il faut entrer les codes prévus par la Statec pour représenter les données Intrastat. Si les codes en question vous sont connus, vous pouvez les entrer à la main, sinon appuyez sur **F3** pour les choisir dans la liste.

Comme c'était déjà mentionné plus haut, le paramétrage pour l'achat et la vente se fait de façon identique, seulement pour l'achat le champ **Pays de destination** est remplacé par les deux champs **Pays d'origine et Pays de provenance** dont le premier correspond au pays de production de la marchandise et le deuxième correspond au pays par lequel la marchandise a passé la frontière pour entrer au Luxembourg. Code tarif douanier: tous les codes tarif douanier se trouvent, pour des raisons de performance et de maniabilité, dans une table externe. Ceci veut dire que, en appuyant sur **F3**, vous ne verrez que les codes tarif qui ont déjà été utilisés auparavant. Pour avoir la liste complète des codes tarif douaniers il faut appuyer simultanément sur les touches "Alt" et **F3**

![](<../.gitbook/assets/image (125).png>)

![](<../.gitbook/assets/image (142).png>)

Pour ajouter un code tarif dans la liste réduite, sélectionnez‐le dans cet écran et cliquez sur **Valider**. Pour rechercher des codes tarifs, vous avez plusieurs outils à votre disposition. Si vous savez dans quel(s) chapitre(s) devrait se trouver le code que vous recherchez, vous pouvez limiter l'affichage à ce(s) chapitre(s). Pour ce faire cliquez sur le bouton **Chapitre**.

![](<../.gitbook/assets/image (68).png>)

Puis sélectionnez‐le ou les chapitres, en cliquant sur la ligne du chapitre, les lignes sélectionnées sont affichées en bleu. Pour désélectionner une ligne cliquez une nouvelle fois sur cette ligne. Quand vous avez fait votre choix, cliquez sur le bouton **Valider** pour continuer.

Vous pouvez aussi effectuer une recherche soit sur le **code tarif**, soit sur la **désignation du tarif**. En appuyant sur la touche **F6**, vous changez entre ces deux modes de recherche. La colonne qui est active pour la recherche est marquée en jaune pâle. Entrez maintenant la clé de recherche au clavier et appuyez sur **Enter**. Les résultats de la recherche seront affichés dans la fenêtre principale. ‐Coef. sup. statistique: Il s'agit là d'un coefficient qui vous permet d'indiquer la valeur statistique d'une marchandise, si cette valeur diffère du montant facturé.

#### **Informations supplémentaires pour les tables clients, fournisseurs et articles**

Les données Intrastat peuvent être encodées dans 7 écrans différents (Voir tableau de l'encodage Intrastat en annexe). Certaines données peuvent être encodées simultanément dans plusieurs écrans, d'autres seulement dans un seul. D'une manière générale, plus la portée de l'écran où vous encodez les données est grande (p.ex. **Paramètres dossier**), plus la priorité des données est petite.

Si par exemple vous avez indiqué dans les paramètres du dossier comme pays de provenance par défaut la Belgique, cette valeur sera proposée lors de l'encodage Intrastat si vous n'avez pas indiqué de pays de provenance ni pour le fournisseur ni pour les articles du document d'achat à traiter. Si par contre vous faites une commande auprès d'un fournisseur allemand et que vous avez encodé le pays de provenance dans les données de base de ce fournisseur, le programme va proposer comme pays de provenance l'Allemagne.

#### **La table des articles**

Les données encodées dans cette table seront considérées en premier lieu par le programme pour le remplissage automatique des formulaires. Il est conseillé de n'entrer, pour un article donné, que les valeurs qui sont les plus spécifiques que possibles à ce niveau, comme par exemple le **poids**, ou le **code tarif douanier**. Si vous avez organisé vos articles en **familles, groupes et sous‐groupes** vous pouvez même attribuer le **code tarif douanier** à un tel regroupement d'articles. Dans ce cas vous ne devez pas spécifier le code tarif au niveau de l'article mais au niveau plus général (**famille/groupe/sous-groupe**).

![](<../.gitbook/assets/image (163).png>)



Les champs 1‐3, 6‐9 et 10 ont déjà été décrits dans la partie "Paramétrage du dossier" de ce chapitre. \* **Poids**: Il faut indiquer ici la masse nette en kilogrammes par unité d'article. Certains codes tarifs douaniers prévoient une unité statistique supplémentaire, dans ce cas l'indication du poids est facultative. _Le poids de l'article est à entrer avec décimales. Lors de la génération du rapport Intrastat, le poids cumulé des articles ayant le même tarif douanier sera arrondi._ \* **Quantité supplémentaire**: Entrez ici la quantité pour l'unité statistique supplémentaire. Cette unité, qui est requise pour certains codes tarif, est affichée automatiquement si soit l'article, soit sa famille/groupe/sous‐groupe est déjà associé à un code tarif douanier.

* Proposition du poids/quantité supplémentaire. pour les factures achat/vente: Dans les cas où il est difficile de déterminer le poids par unité d'article, vous pouvez entrer dans les champs 11‐13 ou 14‐16 le rapport valeur/poids ou valeur/qté‐suppl. du dernier document d'achat ou de vente. Le programme calculera alors le poids ou la quantité supplémentaire par unité d'article. Ce rapport sera mis à jour automatiquement lors de la création de documents d'achat ou de vente.

![](<../.gitbook/assets/image (132).png>)

![](<../.gitbook/assets/image (166).png>)

#### **La table client / fournisseur**

Il est encore important de vous rappeler, à cet endroit, que les clients/fournisseurs doivent être du type 1. (Intracommunautaire) pour que leurs documents d'achat/vente soient traités par le module Intrastat. Vous pouvez vérifier le type sur la page d'onglet n°2. (Compta) _Pour avoir plus d'informations sur les types des clients veuillez consulter le chapitre II.2.b (Signalétique clients) page 38._

Les données Intrastat que vous entrez au niveau du client/fournisseur ne seront utilisées que si vous n'avez pas encodé ces données pour les articles contenus dans le document de vente/achat. Dans cette perspective il est aussi conseillé de ne remplir que les champs qui ne vont pas changer souvent pour un tel client ou fournisseur.

![](<../.gitbook/assets/image (35).png>)



* Les champs qui sont à remplir dans cet écran ont déjà été décrits auparavant dans la partie "Paramétrage du dossier" de ce chapitre.
* Le pays de destination de la marchandise pour un client donné est repris dans le champ **18. Code pays** de la signalétique du client.
* Le pays de provenance et le pays d'origine de la marchandise sont repris dans le même champ **18. Code pays** de la signalétique du fournisseur.

### La gestion des documents intrastat <a href="#la-gestion-des-documents-intrastat" id="la-gestion-des-documents-intrastat"></a>

Vous pouvez gérer les documents d'achat et de vente qui sont pris en compte pour la déclaration Intrastat dans l'écran 18 - Intrastat.

![](<../.gitbook/assets/image (13).png>)

Avant de commencer avec l'encodage, il faut sélectionner une période Intrastat. Par défaut le programme sélectionne la période Intrastat qui contient la date actuelle. Si vous voulez encoder dans une autre période Intrastat, cliquez sur le texte (en bleu souligné) **Période de la déclaration**. Vous aurez la liste des périodes Intrastat disponibles. Sélectionnez une période et cliquez sur le bouton **Valider**. Une fois la période choisie, vérifiez si vous avez bien sélectionné le **type** de documents (achat/vente) que vous voulez traiter. Maintenant il faut choisir le document pour lequel vous voulez traiter les données. Choisir le document pour lequel vous voulez traiter les données Intrastat. Pour faciliter la recherche, vous pouvez vous faire afficher les documents selon les critères suivants:

![](<../.gitbook/assets/image (73).png>)

Ceci vous permet non seulement de voir rapidement ce qui a déjà été traité ou non, mais vous pouvez aussi revoir les documents déjà traités et corriger les données encodées, si nécessaire.

Si vous cliquez sur un des documents qui se trouvent dans la **zone des documents**, vous allez voir le détail des lignes de ce document dans la **zone de détail document**. De cette façon vous pouvez vérifier tout de suite si vous avez sélectionné le bon document. De même si vous cliquez du bouton droit de la souris sur un des documents, un petit menu s'ouvre et vous pouvez choisir entre **Ajouter/modifier les données Intrastat** de ce document et **Aperçu document**. Si vous choisissez **Aperçu document** le programme affichera l'écriture originale de ce document. Dans le cas d'un document de vente ce serait la facture qui sera affichée. Consulter, imprimer et envoyer les déclarations Intrastat.

![](<../.gitbook/assets/image (155).png>)



* Vous pouvez à tout moment jeter un coup d'œil sûr, ou imprimer une déclaration Intrastat pour une période Intrastat précise. Pour ce faire, sélectionnez la période comme décrit plus haut, puis cliquez sur un des boutons **Aperçu** ou **Imprimer** qui se trouvent en haut à droite de l'écran 18.(Intrastat) pour lancer la fonction désirée. En cliquant sur le bouton **Envoyer**, une copie de la déclaration Intrastat actuelle sera envoyée par mail au Statec.

#### **L’ENCODAGE INTRASTAT**

En fonction de ce que vous avez spécifié dans les paramètres du dossier (voir plus haut) pour le mode d'encodage, vous avez plusieurs possibilités pour accéder à l'écran d'encodage des données Intrastat. Si vous avez choisi une des options suivantes: **Pendant l'encodage et A la fin de l'encodage**, l'écran d'encodage Intrastat se présentera automatiquement pour les documents qui nécessitent l'encodage Intrastat. Dans tous les cas vous pouvez accéder aux données Intrastat pour un document dans l'écran **18 Intrastat** qui a été décrit plus haut. Il suffit de choisir le document désiré et de double‐cliquer sur ce document dans la « zone des documents ». Cet écran va apparaître:

![](<../.gitbook/assets/image (160).png>)

avez paramétré votre dossier en vue d'un encodage automatique des données Intrastat et que vous avez complété vos enregistrements clients, fournisseurs, articles, etc. avec les données Intrastat comme c'est décrit dans les paragraphes précédents, alors le programme vous proposera les écritures Intrastat pour les documents où un encodage Intrastat est requis. Dans cette perspective l'écran d'encodage Intrastat sert principalement à vérifier ou à compléter les écritures proposées par **azur**. La zone des lignes Intrastat vous affiche les lignes qui ont déjà été encodées soit par vous‐même, soit par le générateur automatique d'**azur**. Vous pouvez ajouter, modifier ou supprimer des lignes dans la zone des lignes Intrastat en utilisant le groupe de boutons qui est située juste en dessous de cette zone.

#### **AJOUTER UNE LIGNE**

Cliquez sur le bouton **Ajouter ligne**, pour qu’une nouvelle ligne s'ajoute dans la zone des lignes. Cette ligne est déjà pré remplie par les valeurs Intrastat encodées dans les paramètres du dossier et dans la page Intrastat du client/fournisseur actuellement sélectionné. Le masque d'encodage des lignes devient accessible.

![](<../.gitbook/assets/image (141).png>)

Les zones obligatoires (encadrés en rouge) changent en fonction du type de déclaration (simplifiée/détaillée) que vous devez remplir. Le champ **No article** est facultatif. Si vous avez complété les enregistrements des articles avec les données Intrastat, alors ces données seront inscrites automatiquement lorsque vous indiquez le n° de l'article dans une ligne Intrastat. Si tous les champs obligatoires sont remplis vous pouvez cliquer sur le bouton **Ligne OK** pour valider les données entrées. Si vous ne voulez pas garder les ajouts, vous pouvez cliquer sur le bouton **Annuler ligne**.

#### **MODIFIER UNE LIGNE**

Si vous voulez modifier une ligne Intrastat, sélectionnez la ligne dans la zone des lignes et cliquez sur le bouton **Modifier ligne**. Vous pouvez ensuite modifier les valeurs dans le masque d'encodage. Pour garder les modifications cliquez sur **Ligne OK**. Si vous voulez annuler les modifications cliquez sur **Annuler ligne**, dans ce cas la ligne ne sera pas supprimée, seulement les modifications ne seront pas enregistrées.

#### **SUPPRIMER UNE LIGNE**

Pour supprimer une ligne, cliquez sur la ligne à supprimer, puis cliquez sur le bouton **Supprimer ligne**. L'indicateur suivant affiche toujours le montant du document qui n'a pas encore été encodé dans Intrastat. Vous pouvez valider l'Intrastat même si le montant qui reste à comptabiliser est non nul. Ceci n'est à conseiller que pour des exceptions, comme par exemple si un document de vente contient aussi bien des marchandises à déclarer que des services facturés qui ne sont pas à déclarer. Quand vous aurez terminé l'encodage Intrastat pour le document en cours vous pouvez cliquer sur le bouton **Valider Intrastat**. Ceci a comme effet que les données encodées seront sauvegardées, le document sera marqué comme déjà encodé dans Intrastat et les données des lignes seront ajoutées à la déclaration Intrastat de la période sélectionnée. Pour supprimer toutes les lignes déjà encodées dans l'écran actuel dans le but de refaire tout l'encodage pour le document sélectionné, cliquez sur le bouton **Vider Intrastat**. Si vous voulez recommencer l'encodage en vous basant sur la proposition automatique, cliquez sur le bouton **Reproposé Intrastat**. Si vous ne voulez pas que le document actuel soit pris en compte par la déclaration automatique d'Intrastat, cliquez sur le bouton **Sans Intrastat**.

**IMPORTANT!** _Cela est définitif, vous n’aurez plus la possibilité d’annuler cette action!_

### Contrôle IBLC <a href="#controle-iblc" id="controle-iblc"></a>

#### **Changement 2021**

Dans la mesure où il le numéro de Tva du partenaire (numéro d’identification Intracommunautaire) doit être ajouté au fichier des expéditions des déclarations Intrastat, nous avons décidé d’ajouter un contrôle sur ces numéros afin de garantir que les fichiers soient de qualité. Cela servira également pour les déclarations Etats récapitulatifs de biens et de Services. La vérification du numéro d'identification intracommunautaire du CLIENT, FOURNISSEUR ou DOSSIER peut être faite de plusieurs manières :

Soit par l'écran dynamique (F5) comme cela se faisait déjà auparavant (1 sur le printscreen).

![](<../.gitbook/assets/image (131).png>)

Soit par le scripteur (Contrôle IBLC - Contrôle numéro d'identification intracommunautaire (IBLC)) par accès direct ou par raccourci vers celui-ci comme par exemple via le bouton « Gestion des N° d’ident. Intracommunautaire … » dans le menu 321 (2 sur le printscreen) ou 331.

![](<../.gitbook/assets/image (113).png>)



{% hint style="info" %}
* contrôler tous les CLIENTs, FOURNISSEURs ou DOSSIERs
* corriger les numéros d'identification intracommunautaire

Ce scripteur vous permet de :

**info**


{% endhint %}

{% hint style="info" %}
**Tip**



* Cliquer sur le type de contrôle que vous voulez effectuer (Client, Fournisseur, Dossier).
* Cliquer sur les ensembles sur lesquels vous voulez effectuer le contrôle (vous pouvez en sélectionner/désélectionner plusieurs et ceux-ci passent en vert s’ils sont cliqués/dans votre sélection) : « Pas contrôlé (?) », « Contrôlé ok (V) » , « Contrôlé KO (X) »
* Cliquer sur le type de contrôle ou d’action/correction que vous voulez effectuer sur votre sélection globale en bas : « Nettoyer N° », « Contrôler Tout », « Contrôler Ligne », « Propose Pays Ligne »
*

:warning: **Warning**

* Attention, le code pays doit être intégré dans le numéro présent pour pouvoir être contrôlé : il est possible d'ajouter le code pays au numéro avec la fonction "Propose Pays Ligne"
* seul les espaces sont tolérés : il est possible de lancer un nettoyage de tous les numéros pour remplacer les caractères / . , - : par un espace avec la fonction "Nettoyer N°"
{% endhint %}

![](<../.gitbook/assets/image (135).png>)

Dans l'écran dynamique Client 321 et Fournisseur 331, une image (drapeau de l'Europe) représentant le statut de la vérification est affichée:

avec un V vert pour dire que le numéro est Valide

![](<../.gitbook/assets/image (11).png>)

avec un X rouge pour dire que le numéro a été testé et qu'il n'est pas Valide

![](<../.gitbook/assets/image (25).png>)

avec un ? orange pour dire que le numéro n'a pas été testé sans se prononcer sur sa validité

![](<../.gitbook/assets/image (92).png>)

Dans l'écran de l'intrastat, le numéro d'identification intracommunautaire a été ajouté dans la liste des documents ainsi que le statut (toujours représenté par l'image).

![](<../.gitbook/assets/image (74).png>)

Dans l'écran d'encodage, le numéro, le nom, le numéro d'identification intracommunautaire et le statut représenté par l'image a été ajouté en haut dans un panel.

![](<../.gitbook/assets/image (28).png>)

La saisie du code pays d'origine a été rendu obligatoire pour les expéditions.

Lors de l'édition d'un rapport d'intrastat d'Expédition, si des numéros d'identifications intracommunautaires utilisés ne sont pas vérifiés, un message vous en informera et vous pourrez alors ouvrir un report des partenaires concernés afin de les valider (pas obligatoire, vous pouvez déposer un fichier avec des numéros vides ou pas contrôlés sous votre responsabilité).

![](<../.gitbook/assets/image (14).png>)

![](<../.gitbook/assets/image (27).png>)

Dans les fichiers d'export, le code pays d'origine a été ajouté pour les expéditions.

Dans les fichiers d'export le numéro d'identification intracommunautaire a été ajouté à la fin du fichier, il est rempli pour les expéditions et laissé vide pour les arrivées. Dans l’application Idep.Web, vous devez utiliser à partir de 2021 le nouveau format « AZUR Sita 2021 » qui contient le champ Devise et Numéro TVA partenaire en plus de l’ancien format (AZUR Sita Software).

![](<../.gitbook/assets/image (82).png>)

### Module état récapitulatifs <a href="#module-etat-recapitulatifs" id="module-etat-recapitulatifs"></a>

#### **Changement 2021**

Les mêmes contrôles ont été ajoutés dans les Etat récapitulatifs (Livraisons de biens et Prestations de services), c'est-à-dire si des numéros d'identifications intracommunautaires utilisés ne sont pas vérifiés, vous recevrez un message pour vous en informer et vous pourrez alors ouvrir un report des partenaires concernés afin de les valider. Il n’y a pas d’obligation, vous pouvez tout de même valider la déclaration sous votre responsabilité). Si vous choisissez de la rendre définitive, vous recevrez juste un message comme quoi ce n’est pas conseillé.

![](<../.gitbook/assets/image (59).png>)
