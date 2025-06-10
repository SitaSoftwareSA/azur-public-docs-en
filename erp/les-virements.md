# Les virements

### Introduction <a href="#introduction" id="introduction"></a>

Le module « Virements » d'Azur a été conçu pour préparer les ordres de virement qui vont être envoyés à travers le programme « Multiline » de l'ABBL. Azur vous propose, selon vos critères de sélection, les paiements à effectuer. Après avoir validé cette sélection, Azur crée un fichier texte dans le format prévu par Multiline.

{% hint style="danger" %}
Warning

Avant tout, il faut encoder les comptes en banque de votre société dans azur. Ceux-ci doivent être enregistrés dans trois endroits différents. À savoir, dans les programmes respectifs:

* '341.' Table des comptes généraux en tant que compte financier
* '31.' Paramètres dossier: dont les données doivent être définies accordement comprenant limite de crédit, nom du détenteur du compte etc...).
* '3D3– Journal des opérations financières' :dans lequel il faut créer un journal financier correspondant et lier le compte financier et le compte en banque dossier à ce journal
{% endhint %}

Si vous encodez déjà vos opérations financières dans le programme 13. Opérations financières vous n'avez plus besoin de créer les comptes financiers, ni les journaux financiers correspondants. Vous pouvez donc passer à l'étape [Création de virements](https://docs.sitasoftware.lu/erp/fr/virement.fr/#creation-des-virements).

### Création d'un compte financier <a href="#creation-dun-compte-financier" id="creation-dun-compte-financier"></a>

* Aller dans le programme 31. Paramètre du dossier
* Onglet 6. Banque, cliquer sur Compte en banque

![](<../.gitbook/assets/image (213).png>)

![](<../.gitbook/assets/image (272).png>)

{% hint style="warning" %}
Tip

Le n° de l'onglet pourrait être différent.
{% endhint %}

### Configuration comptes bancaires fournisseurs <a href="#configuration-comptes-bancaires-fournissuers" id="configuration-comptes-bancaires-fournissuers"></a>

Dans le programme 3G "Traitement comptes fournisseurs", vous pouvez creer les comptes bancaires fournisseur en les associant à une banque qui existe.

![](<../.gitbook/assets/image (178).png>)

{% hint style="info" %}
Info



* 1 Code Compte, dans ce champ veuillez saisir un nom/numéro qui identifera ce compte pour le fournisseur.
* 2 Numéro du fournisseur
* 3 Code banque = le code de la banque (si le code n'existe pas, vous pouvez le créer via le programme "3C Table des codes banques") [Plus d'infos](https://docs.sitasoftware.lu/erp/fr/virement.fr/#creation-de-banques)
* 4 N° de compte banque IBAN = N° du compte du fournisseur
* 6 Code payement, veuillez mettre VIR
* 7 Etat, veuillez mettre 0

Remarques: Les champs sous **Adresse** ne sont qu'à rentrer si l'adresse du détenteur du compte diffère de celle du fournisseur.
{% endhint %}

### Configuration du fournisseur <a href="#configuration-du-fournisseur" id="configuration-du-fournisseur"></a>

![](<../.gitbook/assets/image (179).png>)

{% hint style="info" %}
Info

* 8 Mode de paiement, VIR
* 9 Code du compte = compte créé au point [Configuration comptes bancaires fournissuers](https://docs.sitasoftware.lu/erp/fr/virement.fr/#Configuration-comptes-bancaires-fournisseurs)
* 10 N° compte = N° du compte fournisseur, champ utilisé uniquement pour les imports. Ce champ n'est pas utilisé pour les virements. Azur va voir dans les comptres bancaires fournisseurs.
{% endhint %}

### Création de banques <a href="#creation-de-banques" id="creation-de-banques"></a>

![](<../.gitbook/assets/image (251).png>)

{% hint style="info" %}
Info



* 1 Code de la banque, ce code est un code formaté
* 2 Nom de la banque
* 13 Code, est composé de 4 LETTRES
* 14 Code pays, est composé de 2 LETTRES
* 15 Ville est composé de 2 LETTRES

Remarques: Code de la banque (1.)= Code(13.) + Code Pays(14.) + Ville(15.) BGLLLULL = BGLL + LU + LL
{% endhint %}

{% hint style="warning" %}
Tip

Au cas où vous devez créer une banque étrangère dans azur, vous devez vous assurer que vous disposez soit du code:



* SWIFT code
* d'un code banque tel que Code RIB, AT, BLZ, etc.
* ainsi que du nom et de l'adresse de la filiale\
  En visitant le site [www.swift.com](http://www.swift.com/) vous pouvez éventuellement compléter les informations manquantes.
{% endhint %}

### Création du journal financier / lire les comptes à partir d'un journal <a href="#creation-du-journal-financier-lire-les-comptes-a-partir-dun-journal" id="creation-du-journal-financier-lire-les-comptes-a-partir-dun-journal"></a>

Pour achever cette partie, nous avons encore besoin d'un journal financier par compte. Veuillez démarrer le programme "3D3. Journal des opérations financières"

![](<../.gitbook/assets/image (229).png>)

### Création des virements <a href="#creation-des-virements" id="creation-des-virements"></a>

Démarrez le programme "42. Création virements" et cliquez sur l'onglet Paramètres virements.

![](<../.gitbook/assets/image (243).png>)

L'écran se présente alors de la façon suivante:

![](<../.gitbook/assets/image (223).png>)

Azur peut générer automatiquement les textes qui seront affichés dans les lignes de la communication du virement. Azur reprend des informations concernant la facture, comme par exemple, la date ou le numéro. Comme il n'y a que 4 lignes à 35 caractères (par virement par bénéficiaire), il faudra indiquer au programme le nombre de factures pour lesquelles les informations détaillées seront affichées dans la communication. S'il y a plus de factures pour un même bénéficiaire, un autre texte (que vous pourrez spécifier à un autre endroit) sera affiché dans le champ **Communication du virement**.

Le paramétrage de ces textes sera expliqué plus loin dans cette documentation. Par défaut ce nombre est fixé à 3, il reste alors une ligne de la référence pour afficher des informations comme par exemple le numéro d'ordre de virement.

{% hint style="info" %}
Info

Les codes frais pour les virements (LUP)



* BEN =Bénéficiaire
* OUR = Donneur d'ordre
* SHA= Partagés Les codes frais pour les domiciliations (LSL):
* DEB = Débiteur
* CRE = Créditeur
{% endhint %}

Les textes figurant dans les champs **Identification pour virements** seront envoyés à la banque (fichier LUP) respectivement à la CETREL (fichier LSL) avec les fichiers Multiline. L'identification pour les banques doit contenir un nom court (16 caractères) pour votre société. Si vous faites des domiciliations avec Azur, vous devez mettre le code à 10 chiffres qui vous a été donné par la Cetrel. Après avoir modifié des paramètres vous devez cliquer sur le bouton **Sauvegarder** dans la partie inférieure gauche de l'écran. Pour configurer les textes générés pour les lignes de la communication vous devez cliquer sur l'onglet **Textes par défaut**.

![](<../.gitbook/assets/image (237).png>)

En cliquant sur le bouton **Recherche**, le programme va afficher les textes existant pour la combinaison de paramètres (Code langue, client ou fournisseur, type fichier, etc.) que vous avez choisie.

Pour modifier par exemple le texte qui sera affiché dans la première ligne de la communication d'un ordre de virement, vous devez double-cliquer sur **Ligne référence no.1**

![](<../.gitbook/assets/image (241).png>)

Il s'agit ici d'un évaluateur de fonctions, c'est-à-dire un assistant qui vous permet de construire des chaînes de texte et de les formater selon certains critères. Exemple: Si vous voulez que le programme prenne le texte se trouvant dans la référence de la facture, qu'il mette ce texte en lettres majuscules en rajoutant le texte 'Réf.:' devant, qu'il rajoute des espaces derrière pour arriver à une longueur totale de 20 caractères et enfin qu'il découpe si le texte résultant dépasserait les 20 caractères. La formule résultante sera la suivante: **AjouteCharDevDer('Réf.:'+{REFERENCE},' ',20,True)**

{% hint style="info" %}
**Info**

L'élaboration de ces formules dépasse le cadre de ce chapitre et sera expliquée ailleurs en détail.
{% endhint %}

### La création du fichier virement <a href="#la-creation-du-fichier-virement" id="la-creation-du-fichier-virement"></a>

Une fois que vous avez paramétré votre dossier pour les virements, vous pouvez passer à la création des virements via le programme **42. Création virements**.

![](<../.gitbook/assets/image (225).png>)

Le programme fait la distinction entre deux catégories de bénéficiaires qui sont les clients et les fournisseurs. Pour les fournisseurs, vous ne disposez que du type fichier 'LUP' pour les virements, tandis que pour les clients, il est autant possible de réaliser des virements (fichier LUP) que des ordres de domiciliations (fichier LSL).

### Sélection des factures pour virements <a href="#selection-des-factures-pour-virements" id="selection-des-factures-pour-virements"></a>

{% hint style="warning" %}
**Tip**

Dans les nouvelles versions d'Azur, vous pouvez sélectionner les factures fournisseurs à payer avec escompte via l'onglet **Préparations Virements suivant escompte**
{% endhint %}

![](<../.gitbook/assets/image (247).png>)

### Préparations de virements suivant escompte <a href="#preparations-de-virements-suivant-escompte" id="preparations-de-virements-suivant-escompte"></a>

![](<../.gitbook/assets/image (204).png>)

### **Liste des fournisseurs sélectionnés pour la recherche**

Dans la partie de gauche, vous trouvez la liste des fournisseurs sélectionnés pour la recherche, par défaut, le programme va sélectionner tous les fournisseurs.

![](<../.gitbook/assets/image (268).png>)

### **Liste des banques**

En bas à gauche, vous avez la liste de vos banques depuis lesquelles vous allez pouvoir exécuter les virements.

![](<../.gitbook/assets/image (216).png>)

{% hint style="info" %}
Info

* En bleu la banque active
* Pour passer d’une banque à une autre, vous pouvez utiliser la touche F4.
{% endhint %}

### **Recherche**

![](<../.gitbook/assets/image (208).png>)

### **Partie centrale**

![](<../.gitbook/assets/image (194).png>)

{% hint style="info" %}
**Info**



* La première grille affiche un total par fournisseur.
* La deuxième grille affiche le détail du fournisseur actif dans la première grille.
* La troisième grille affiche le détail de l’escompte du document actif dans la deuxième grille.
{% endhint %}

### Actions

![](<../.gitbook/assets/image (211).png>)



| Actions                          | Descriptions                                                                                                                                                                                                                                     |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Traitement automatique           | Le programme va parcourir l’ensemble des données affichées et si la facture comporte une escompte et qu’il n’a pas encore eu de traitement dessus, le programme va faire un encodage automatique sur la banque active.                           |
| Traitement automatique sélection | Pour chaque fournisseur sélectionné (CTRL + CLICK) dans la première grille, le programme va faire le même traitement que le traitement automatique.                                                                                              |
| Annuler sélection                | Pour chaque fournisseur sélectionné (CTRL + CLICK) dans la première grille, le programme va annuler tout ce qui est saisi.                                                                                                                       |
| Annuler tout                     | Le programme va parcourir l’ensemble des données affichées et annuler tout ce qui est saisi.                                                                                                                                                     |
| Virement sans document           | Permet de préparer un virement sans pour autant spécifer un document Azur ![image creation virement Creation fichier avec escompte sans doc](https://docs.sitasoftware.lu/erp/fr/images/virement_preparation_suivant_escompte_sans_document.png) |
| Montant sans escompte            | Pour le document actif dans la deuxième grille, le programme va faire la saisie du montant sans l’escompte.                                                                                                                                      |
| Montant auto                     | Le programme va faire la saisie automatiquement et va privilégier le montant avec escompte si possible.                                                                                                                                          |
| Montant + Montant Manuel         | Permet d’encoder le montant souhaité pour le document actif dans la deuxième grille.                                                                                                                                                             |
| Annuler                          | Le programme va annuler ce qui est saisi sur le document actif dans la deuxième grille.                                                                                                                                                          |
| DMS                              | Affiche le document dans le DMS si présent.                                                                                                                                                                                                      |
| Litige                           | Affiche les informations de litige si présent.                                                                                                                                                                                                   |
| Visualiser avant validation      | Ouvre un nouvel écran et affiche en détail les fournisseurs qui vont recevoir de l’argent, le montant et la banque utilisée.                                                                                                                     |
| Valider pour virement            | Enfin, la validation qui va permettre à l’utilisateur de retourner dans le 42 (Création virements).                                                                                                                                              |

{% hint style="warning" %}
**Tip**

Le programme 42 reprendra l'ensemble des informations qui viennent d'être saisies et **validées pour virement**.
{% endhint %}
