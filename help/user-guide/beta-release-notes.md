---
title: Notes de mise à jour d’Adobe GenStudio for Performance Marketing Beta
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio for Performance Marketing.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: ca83beb4d6f5bd0d79a2da69658b6e18c3252f2e
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# Notes de mise à jour d’Adobe GenStudio for Performance Marketing Beta

Ces notes mettent en évidence d’importants correctifs et améliorations d’Adobe GenStudio for Performance Marketing pour la semaine se terminant le 27 septembre.

## Nouvelles fonctionnalités et améliorations

* GenStudio peut désormais extraire des informations sur les personnages et les produits d’un PDF chargé et renseigner les champs associés. <!-- GS-3806 -->

* Les utilisateurs peuvent désormais filtrer les ressources et expériences [!DNL Content] en fonction du nom de l’utilisateur qui a chargé la ressource. <!-- GS-1808 -->

* La section [!DNL Additional details] a été renommée [!DNL Messaging preferences] dans la page de détails [!DNL Products]. <!-- GS-5133 5134 -->

* Ajout d’un bouton [!DNL Add persona] à la page _Ajouter votre première persona_. <!-- GS-5132 -->

## Problèmes connus

La résolution des problèmes connus suivants est programmée dans la version GA de GenStudio for Performance Marketing.

* Les modèles peuvent être chargés, mais ils ne sont pas visibles. **Solution** : téléchargez une ressource avec le champ **[!UICONTROL Campagnes]** renseigné. Ensuite, chargez à nouveau le modèle. <!-- GS-4815 5650-->

* Les utilisateurs ne peuvent pas recadrer manuellement les métadonnées publicitaires après les avoir redimensionnées. <!-- GS-5871 -->

* Les utilisateurs peuvent créer un [!DNL Campaign] à partir de [!DNL Content] workflows. <!-- GS-5650 -->

* Les utilisateurs doivent se connecter deux fois à un compte Métadonnées de canal lorsqu’ils sont également connectés à Facebook. Solution : déconnectez-vous de Facebook avant de vous connecter à un compte de métadonnées de canal. <!-- GS-3009 -->

### Améliorations supplémentaires et problèmes résolus

* Les problèmes de latence intermittente avec certaines opérations de canevas [!DNL Create] ont été résolus. <!-- GS-5203 -->

* Les utilisateurs n’ont plus besoin de se connecter deux fois à un compte Métadonnées de canal lorsqu’ils sont également connectés à Facebook. <!-- GS-4806 -->

* La génération d’emails entraîne désormais un envoi d’emails incomplet. <!-- GS-5209 -->

* La création d’une campagne dans le workflow de modèle stocke désormais les identifiants comme prévu.  <!-- GS-4923 -->

* Le sélecteur de référentiel multiple répertorie désormais les référentiels par ordre alphabétique. <!-- GS-5553 -->

* Les problèmes liés aux formats de fichiers d’exportation CSV pour les langues autres que l’anglais ont été résolus. <!-- GS-5141 -->

* Les utilisateurs peuvent maintenant cliquer sur le bouton [!DNL Create] _Travail récent_ **[!UICONTROL Afficher tous les brouillons]** pendant le chargement des brouillons. Auparavant, lorsque vous cliquiez sur ce bouton avant le chargement de tous les brouillons, seuls quelques brouillons étaient chargés et le bouton **[!UICONTROL Afficher tous les brouillons]** n’était plus disponible. <!-- GS-3938 -->

* Le canevas [!DNL Create] affiche désormais le bouton **[!UICONTROL Afficher tous les brouillons]** comme prévu lorsque la zone de travail affiche plus de quatre brouillons. <!-- GS-5588 -->

* La recherche fonctionne désormais comme prévu dans l’onglet _Attributs_. <!-- GS-5658 -->

* L’animation Shimmer est désormais mise à l’échelle correctement lors du chargement de l’expérience. <!-- GS-5574 -->

* Les aperçus de miniatures pour les emails en plusieurs parties sont désormais rendus comme prévu dans [!DNL Content]. <!-- GS-5258 -->

* Correction d’un problème lié à Workfront avec le bouton **[!UICONTROL Envoyer pour approbation]**. <!-- GS-5847 -->

* Correction de problèmes liés au chargement du minuscule sur la vue de travail [!DNL Create] récente. <!-- GS-5589 -->

* La saisie d’un terme de recherche entraîne désormais un seul appel de recherche, comme prévu.  <!-- GS-2999 -->

* Correction du rendu des images des métadonnées générées par les publicités après l’exportation. <!-- GS-5749 -->

* Le symbole `%` s’affiche désormais correctement dans les paramètres régionaux DEU, FRA et ESP lorsque les utilisateurs effectuent un zoom avant ou arrière sur les variantes d’emails dans le canevas C[!DNL Create]. <!-- GS-5007 -->


#### Localisation

Cette version comprend des améliorations de la localisation dans l’interface du produit, en particulier dans [!DNL Create]. Les composants d’interface suivants ont été localisés : <!-- GS-5295 -->

* Toutes les chaînes dans la zone _Invite_ (Titre des paramètres, noms des options du menu déroulant et texte de l’espace réservé de l’invite) <!-- GS-5027 -->

* Toutes les chaînes dans la fenêtre _Resize_ pour les métadonnées publicitaires générées dans [!DNL Create] <!-- GS-5035 -->

* Toutes les chaînes dans la zone _Récent travail_ de [!DNL Create] <!-- GS-5037 -->

* Chaînes de l’option de menu déroulant Marques, Personas et Produit dans la zone d’invite <!-- GS-5293 -->

* Chaîne **Zoom pour s’adapter à l’écran** affichée pendant la génération d’un email et d’une méta-publicité <!-- GS-5063 -->

* Formats de date et d’heure, chaîne **Brouillon sans titre** et messages d’erreur dans les noms de message électronique et de métadonnées <!-- GS-5023 5022 5048-->

* L’onglet [!DNL Content] _Assets_ de la galerie d’onglets affiche les chaînes et le symbole de pourcentage (%) <!-- GS-4983 4984-->

* Symbole de pourcentage (%) utilisé dans le taux de clics sur les connaissances > expériences <!-- GS-4279 -->

* Message d’erreur affiché lorsqu’une erreur système se produit lors de la création d’un email ou de métadonnées <!-- GS-5061 -->

* Séparateur décimal de l’expression &quot;Nombre de mots par phrase&quot; sur la page Détails de l’expérience de statistiques <!-- GS-4986 -->

* Chaînes dans le menu Exporter pour une méta-publicité générée avec un modèle. <!-- GS-5031 -->

