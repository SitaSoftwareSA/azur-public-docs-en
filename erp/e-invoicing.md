# e-Invoicing

### Release note <a href="#release-note" id="release-note"></a>



| Lien                                                                                                                                 | Release note                                                                                          | Who | When     |
| ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------- | --- | -------- |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v16-ajout-les-annexes)                                                      | V16: Ajoute les Annexes.                                                                              | MFI | Jan 2022 |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v15-ajoute-annuaire-simple)                                                 | V15: Ajoute un mode annuaire "simple".                                                                | MFI | May 2021 |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v14-ajoute-le-mode-rappel-20)                                               | V14: Intégration du mode Azur Rappel 2.0.                                                             | MFI | May 2021 |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v13-ajoute-la-posssibilite-de-specifier-un-report-azur-par-dossier)         | V13: Ajoute la posssibilité de spécifier un report azur par Dossier.                                  | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v121-ajoute-la-possibilite-de-merger-en-1-seul-fichier-les-fichiers-joints) | V12.1: Ajoute la possibilité de merger les fichiers joints.                                           | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v12-ajoute-la-possibilite-de-voir-dans-lemail-la-liste-des-articles)        | V12: Ajoute la possibilité de voir dans l'email la liste des articles.                                | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v111-choix-de-lemail-copy)                                                  | V11.1: Ajoute la possibilité de spécifier l’adresse email copy qui envoi l’email par type de document | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v11-choix-de-lemail-denvoi)                                                 | V11: Ajoute la possibilité de spécifier l’adresse email qui envoi l’email par type de document        | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#ajoute-la-possibilite-de-joindre-2-fichiers)                                | V10: Ajoute la possibilité de joindre 2 fichiers en « one shot »                                      | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#ajoute-la-possibilite-de-joindre-un-document-source-du-dms)                 | V10: Ajoute la possibilité de joindre un document Source du DMS                                       | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v9-rappel-client)                                                           | V9: Rappel client                                                                                     | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v8-statistique)                                                             | V8: Statistique                                                                                       | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v7-avis-de-paiement)                                                        | V7: Avis de paiement                                                                                  | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v6-ajout-de-la-possibilite-de-joindre-5-fichiers)                           | V6: Ajout de la possibilité de joindre 5 fichiers                                                     | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v5-utilisation-dun-annuaire-dedie)                                          | V5: Utilisation d’un annuaire dédié                                                                   | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v4-ajoute-texte-libre)                                                      | V4: Ajoute texte libre                                                                                | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v3-remplacement-de-texte)                                                   | V3: Remplacement de texte                                                                             | MFI |          |
| [...](https://docs.sitasoftware.lu/erp/fr/einvoicing.fr/#v2-integration-des-sms)                                                     | V2: Intégration des SMS                                                                               | MFI |          |

### Gestion des documents à envoyer par email ou à imprimer <a href="#gestion-des-documents-a-envoyer-par-email-ou-a-imprimer" id="gestion-des-documents-a-envoyer-par-email-ou-a-imprimer"></a>

Ecran principal

![](<../.gitbook/assets/image (342).png>)

Ecran principal à la version 15

![](<../.gitbook/assets/image (341).png>)



Cet écran permet :

* D’envoyer par mail un/des documents Azur
* Et/ou
* D’imprimer un/des documents Azur
* D’avoir un historique  

#### Envoi d’email <a href="#envoi-demail" id="envoi-demail"></a>

**Envoyer 1 email**

Pour envoyer un email :

1. Préparer votre recherche et cliquer sur le bouton Recherche.
2. Positionnez-vous sur le document que vous voulez traiter.
3. Vous avez la possibilité de forcer éventuellement une adresse email
4. Cliquer sur envoyer 1 email

![](<../.gitbook/assets/image (281).png>)

Sur la droite, vous visualisez le log de ce qui se passe.

![](<../.gitbook/assets/image (324).png>)

{% hint style="info" %}
Info

Dans les nouvelles versions, les logs se trouvent sur la gauche de l'écran
{% endhint %}

Une fois l’email envoyé le programme enregistre la date d’envoi de l’email et l’adresse à qui il a été envoyé.

![](<../.gitbook/assets/image (310).png>)

**Envoyer N emails**

Pour envoyer plusieurs emails en même temps :

* Préparer votre recherche et cliquer sur le bouton Recherche.
* Sélectionner tout ou les documents que vous voulez envoyer
* Utiliser le bouton Sélectionner tout
* Faire un CTRL + Click pour sélectionner manuellement les documents à envoyer
* Cliquer sur Envoyer emails selon sélection

#### Impression des documents <a href="#impression-des-documents" id="impression-des-documents"></a>

Le programme vous permet aussi d’imprimer les documents, il enregistre la date d’impression. Si vous ne spécifiez pas d’imprimante, le programme prendra votre imprimante par défaut. Le système de sélection fonctionne de la même façon que pour les emails.

**Layout de l’email**

Pour changer le body, rendez-vous dans le dossier 0, dans le 3k2, type 201 N° 3

{% hint style="warning" %}
Warning

Bien cocher HTML, le n° peut varier selon la configuration.
{% endhint %}

#### V2 Intégration des SMS <a href="#v2-integration-des-sms" id="v2-integration-des-sms"></a>

Texte du sms Rendez-vous dans le dossier 0, 3K2, type 201 n°4  

#### V3 Remplacement de texte <a href="#v3-remplacement-de-texte" id="v3-remplacement-de-texte"></a>

Les textes suivants seront remplacés



| SMS                 | Email sujet | Email body |                      |   |
| ------------------- | ----------- | ---------- | -------------------- | - |
| << NOM \_CLI >>     | x           |            | x                    |   |
| << NO\_DOCUMENT >>  | x           | x          | x                    |   |
| << NOM\_DOCUMENT >> | x           | x          | x                    |   |
| << FILENAME >>      |             |            | x                    |   |
| << TITRE >>         |             |            | Nom type document n° |   |
| << TEXTE\_LIBRE >>  |             |            | x                    |   |
| << ARTICLES >>      |             |            | \*Version 12         |   |

{% hint style="success" %}
Tip

Pas d'espaces
{% endhint %}

#### V4 Ajoute texte libre <a href="#v4-ajoute-texte-libre" id="v4-ajoute-texte-libre"></a>

![](<../.gitbook/assets/image (280).png>)

#### V5 Utilisation d’un annuaire dédié <a href="#v5-utilisation-dun-annuaire-dedie" id="v5-utilisation-dun-annuaire-dedie"></a>

**Nouveauté dans la version 5**

«Configuration de l’annuaire ». Azur Document ne regardera plus la configuration dans le client mais dans l’annuaire de cet écran. Pas de panique, une fonction vous permet d’importer ce qui est déjà encodé dans la table client ( pour les clients actifs).

Dans l’annuaire, vous allez pouvoir spécifier par client, type de document, sous-type de document, type d’adresse et n° d’adresse une adresse email, un n° de téléphone et définir si pour la combinaison une impression doit être faite ou non.

Vous avez la possibilité d’initialiser/importer. Cette action importera vos clients qui ne sont pas encore dans l’annuaire et pour lesquels une adresse email est renseignée dans sa fiche client. Lors de cette importation, les différents paramètres seront initialisés à -1 (pour tous).

![](<../.gitbook/assets/image (306).png>)

![](<../.gitbook/assets/image (340).png>)

#### V6 Ajout de la possibilité de joindre 5 fichiers <a href="#v6-ajout-de-la-possibilite-de-joindre-5-fichiers" id="v6-ajout-de-la-possibilite-de-joindre-5-fichiers"></a>

**Nouveauté : dans la version 6**

Vous pouvez spécifier jusqu’à 5 attachements à joindre dans vos emails

![](<../.gitbook/assets/image (290).png>)



* Allez dans les options et indiquez le nom du fichier pdf à joindre dans les champs prévus à cet effet.
* Les fichiers sont à placer dans le dossier « Email » dans le répertoire d’Azur.
* Cliquer droit sur le raccourci d’Azur, Propriété, Ouvrir l’emplacement du fichier

![](<../.gitbook/assets/image (301).png>)

{% hint style="warning" %}
Warning

Attention, bien spécifier le nom avec son extension.
{% endhint %}

#### V7 Avis de paiement <a href="#v7-avis-de-paiement" id="v7-avis-de-paiement"></a>

**Nouveauté : dans la version 7** Vous pouvez envoyer un avis de paiement depuis le programme 42 (Création virement).

**Avantage** : Lorsque vous faites un virement de plusieurs factures à un fournisseur, il nous est impossible de mentionner toutes les factures. En utilisant l’avis de paiement, vous allez pouvoir informer votre fournisseur (par courrier ou par email) de la liste de factures payées.

Préalablement rendre votre proposition de virement définitive. Une fois la proposition rendue définitive, un nouvel onglet apparait « Avis de paiement ».

![](<../.gitbook/assets/image (335).png>)

Cliquez sur Avis de paiement pour ouvrir l’écran de gestion des emails.

![](<../.gitbook/assets/image (297).png>)

Chargez le fichier avec le bouton « Mode virement ». Ensuite vous pouvez le traiter comme un document «normal ». Le report utilisé est spécifique à cette partie et est configurable dans les paramètres de l’écran. Ci-dessous un exemple de document généré.

![](<../.gitbook/assets/image (287).png>)

#### V8 Statistique <a href="#v8-statistique" id="v8-statistique"></a>

**Nouveauté** : dans la version 8, vous pouvez visualiser un total des lignes qui sont affichées dans la grille principale.

**Avantage** : plus besoin d’aller dans le programme « Impression des documents de ventes » pour avoir des totaux.

![](<../.gitbook/assets/image (291).png>)

#### V9 Rappel client <a href="#v9-rappel-client" id="v9-rappel-client"></a>

**Nouveauté** : dans la version 9, vous pouvez envoyer un rappel par email, ou l’imprimer, le tout générer avec un rapport d’azur Reporting Version2.

**Avantages** :

* Optimisation des processus
* Paperless, vous pouvez envoyer les rappels par email
* Traçabilité, vous stocker automatiquement le rappel de votre client dans son DMS

Préalablement faites vos rappels depuis le programme 21 comme vous avez toujours fait. Ouvrez ensuite le programme Azur documents Cliquer sur importer Rappel (Dans la version 9, le programme importera le dernier lots de rappel que vous venez de générer, dans une version ultérieur, vous serez invité à choisir le lot de rappel que vous voulez traiter).

![](<../.gitbook/assets/image (317).png>)

Une fois le fichier importé, vous recevez un message de confirmation et vous pouvez visualiser dans les logs ce qui se passe.

![](<../.gitbook/assets/image (300).png>)

Un service va automatiquement traiter ce fichier.

![](<../.gitbook/assets/image (327).png>)

Ci-dessus, le message qui indique que le service vient de démarrer ![eInvoicing V9 4](https://docs.sitasoftware.lu/erp/fr/images/einvoicing_ecran_v9_4.png) Enfin le message qui vous prévient que le service a fini de traiter le lot de rappel

Sélection Rappel en haut de l’écran et cliquer sur rappel. Vous pouvez à présent traiter vos rappels comme vos autres documents.

![](<../.gitbook/assets/image (343).png>)

Le fichier est aussi présent dans le DMS du client !

![](<../.gitbook/assets/image (349).png>)

#### V10 <a href="#v10" id="v10"></a>

**Ajoute la possibilité de joindre 2 fichiers**

Ajoute la possibilité de joindre maximum 2 fichiers à votre email envoyé

![](<../.gitbook/assets/image (284).png>)

**Ajoute la possibilité de joindre un document Source du DMS**

Sélectionnez une ou plusieurs lignes dans la grille de droite pour envoyer le document DMS lié comme pièce jointe à votre email. Ne fonctionne que pour l’envoi d’un email à la fois

#### V11 Choix de l’email d’envoi <a href="#v11-choix-de-lemail-denvoi" id="v11-choix-de-lemail-denvoi"></a>

Dans les options de l’écran, l’utilisateur a maintenant la possibilité de spécifier une adresse email d’envoi par type de document.

![](<../.gitbook/assets/image (318).png>)

**V11.1 Choix de l’email copy**

#### V12 Ajoute la possibilité de voir dans l’email la liste des articles <a href="#v12-ajoute-la-possibilite-de-voir-dans-lemail-la-liste-des-articles" id="v12-ajoute-la-possibilite-de-voir-dans-lemail-la-liste-des-articles"></a>

Vous pouvez activer désactiver cette option dans l’écran de configuration dans la rubrique « Tableau article ».

![](<../.gitbook/assets/image (305).png>)

Ce qui peut donner l’email ceci:

![](<../.gitbook/assets/image (276).png>)

#### V12.1 Ajoute la possibilité de merger en 1 seul fichier les fichiers joints <a href="#v121-ajoute-la-possibilite-de-merger-en-1-seul-fichier-les-fichiers-joints" id="v121-ajoute-la-possibilite-de-merger-en-1-seul-fichier-les-fichiers-joints"></a>

![](<../.gitbook/assets/image (312).png>)

#### V13 Ajoute la posssibilité de spécifier un report azur par Dossier. <a href="#v13-ajoute-la-posssibilite-de-specifier-un-report-azur-par-dossier" id="v13-ajoute-la-posssibilite-de-specifier-un-report-azur-par-dossier"></a>

![](<../.gitbook/assets/image (322).png>)

#### V14 Ajoute le mode Rappel 2.0 <a href="#v14-ajoute-le-mode-rappel-20" id="v14-ajoute-le-mode-rappel-20"></a>

![](<../.gitbook/assets/image (282).png>)

#### V15 Ajoute annuaire simple <a href="#v15-ajoute-annuaire-simple" id="v15-ajoute-annuaire-simple"></a>

![](<../.gitbook/assets/image (319).png>)



* Avec l’annuaire simple, il est maintenant plus facile de voir et de définir la/les adresse(s) emails pour un client.
* Ajout des zones email cc et email Bcc

#### V16 Ajout les Annexes <a href="#v16-ajout-les-annexes" id="v16-ajout-les-annexes"></a>

![](<../.gitbook/assets/image (313).png>)



* Ajout du type document Annexe (11).
