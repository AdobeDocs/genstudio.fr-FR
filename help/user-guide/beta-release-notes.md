---
title: Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio pour les marketeurs de performance.
source-git-commit: 16f44baf646d696da3572ac2c17a5efb7c8f7fc6
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---


# Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta

Ces notes mettent en évidence un Adobe GenStudio important pour les correctifs et améliorations des marketeurs de performance pour la semaine se terminant le 6 septembre.

## Problèmes connus

Les problèmes connus suivants sont programmés pour la résolution dans la version GA de GenStudio pour les marketeurs de performance.

* Les éditeurs rencontrent parfois un message d’erreur &quot;Une erreur s’est produite&quot; sur le [!DNL Create Canvas] lors de la génération de l’image. **Solution** : si l’erreur se répète, l’utilisateur peut se déconnecter, puis se reconnecter à GenStudio et régénérer l’image.  <!-- GS-4813 -->

* Le [!DNL Create Canvas] effectue un rendu incorrect des images dans les métadonnées publicitaires. <!-- GS-4864 -->

* Assets sans campagnes peut être transféré dans [!DNL Content], mais les utilisateurs peuvent ne pas être visibles. <!-- GS-4815 -->

* Il existe une différence entre les aperçus du canevas de métadonnées et les vues exportées. <!-- GS-4492 4401 -->

* Les miniatures de campagne sont absentes de [!DNL Insights]. <!-- GS-4648 -->

* Les utilisateurs peuvent actuellement sélectionner de petites ressources qui nécessitent un redimensionnement, mais l’agrandissement de ces ressources n’est pas pris en charge. <!-- GS-3131 -->

* Les utilisateurs doivent se connecter deux fois à un compte Meta Ads de canal lorsqu’ils sont également connectés à Facebook. **Solution** : déconnectez-vous de Facebook avant de vous connecter à un compte de métadonnées de canal.

### Résolution de problèmes connus

* GenStudio affiche une erreur lorsqu’un utilisateur tente de saisir des informations d’identification dans la vue [!DNL Insights]. (fixe 8/29) <!-- GS-4689 -->

## Versions Beta précédentes

Les versions précédentes de Beta incluaient les mises en évidence et correctifs suivants.

### Tons clairs

* **Score de validation basé sur le pourcentage** : la validation de marque affiche désormais le score de validation de marque sous forme de pourcentage plutôt qu’une valeur de réussite/échec. (fixed 8/16)

* **Interface d’extraction de marque mise à jour** : l’extraction de marque affiche désormais la fin du processus d’extraction sous forme de pourcentage. (fixed 8/16)

* **Chargement incrémentiel de la marque lors de l’extraction** : les directives de marque sont désormais chargées de manière incrémentielle dans l’interface utilisateur. (fixed 8/16)

* **Création d’emails multi-section** : les utilisateurs peuvent désormais créer des emails composés d’éléments distincts pour le titre, l’image, le corps et CTA. (fixed 8/16)

* **Redimensionnement des métadonnées publicitaires** : les éditeurs peuvent redimensionner les proportions des métadonnées publicitaires. (fixed 8/16)

* **Comptes de connexion de statistiques limités** : la connexion de statistiques ne prend désormais en charge qu’un seul compte par client. (fixed 8/16)

### Améliorations supplémentaires et problèmes résolus

* Le nom d’emplacement du flux de page _Détails de l’expérience_ spécifie désormais le flux Facebook ou Instagram. (fixed 8/16)

* Le recadrage d’images et de vidéos plus grandes est désormais cohérent lorsque l’utilisateur navigue de la vue _Présentation de la ressource_ vers la vue _Détails de la ressource_. (fixed 8/16)

* Le nombre de résultats de recherche sur l’écran Attributs n’affiche plus `0 of` avant qu’un utilisateur ne se connecte. (fixe 8/16) <!-- GS-3665 -->

* Cliquer sur le champ de comptage **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** n’efface plus les paramètres de recherche et de filtre. (fixe 8/16) <!-- GS-3476 -->

### Problèmes connus résolus dans les versions précédentes de Beta

* Le téléchargement des directives sur la marque échoue en raison de problèmes liés à la plateforme de stockage ACP. (fixe 8/22) <!-- GS-4369 -->

* Le menu déroulant Zone d’invite [!DNL Brands] affiche un compteur à la fin de la liste [!DNL Brands] lors de la création de l’email. (fixe 8/22) <!-- GS-4077 -->

