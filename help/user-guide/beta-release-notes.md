---
title: Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio pour les marketeurs de performance.
source-git-commit: f30eaea46a0cbb45f1ba04e393219b843c356e10
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta

Ces notes mettent en évidence un Adobe GenStudio important pour les correctifs et améliorations des marketeurs de performance pour la semaine se terminant le 30 août.

## Tons clairs

* Les directives relatives aux canaux Instagram et Facebook ont été combinées dans les directives relatives aux métadonnées de marque.

* Les éléments de navigation Créer un canevas ont été rationalisés. La page d’entrée ([!DNL Create]) affiche le panneau de navigation de gauche, mais les utilisateurs utilisent désormais un bouton **[!UICONTROL Précédent]** pour accéder à cet espace à partir d’autres zones de travail Créer .  <!-- GS-1189 -->

* Les éléments de navigation ont été améliorés afin de prendre en charge la cible d’action des utilisateurs lors de l’exécution de tâches dans l’ensemble du produit, y compris dans les zones suivantes :

   * Ressource, expérience, détails du modèle dans ([!DNL Content])
   * Expérience, Ressource, Détails des attributs dans ([!DNL Insights])
   * Détails de la marque dans ([!DNL Brands])
   * Détails des produits et personnages dans ([!DNL Products]) et ([!DNL Personas]) <!-- GS-1189 -->

* Les utilisateurs n&#39;ont plus besoin de cliquer sur le bouton **[!UICONTROL Actualiser]** pour afficher les mises à jour des expériences dans ([!DNL Content]). <!-- GS-4218 -->

* La page Détails de l’expérience effectue désormais le rendu des miniatures de ressources externes en tant qu’HTML. <!-- GS-3092 -->

* La latence de l’interface utilisateur après l’ajout ou la suppression d’Assets et d’expériences a été améliorée. <!-- GS-3389 -->

* Les aperçus de modèle incluent désormais un texte par défaut plus explicite. <!-- GS-4028 -->

## Problèmes connus

Les problèmes connus suivants sont programmés pour la résolution dans la version GA de GenStudio pour les marketeurs de performance.

* Il existe une différence entre les aperçus du canevas de métadonnées et les vues exportées. <!-- GS-4492 4401 -->

* Les miniatures de campagne sont absentes de la vue ([!DNL Insights]). <!-- GS-4648 -->

* Les utilisateurs peuvent actuellement sélectionner de petites ressources qui nécessitent un redimensionnement, mais l’agrandissement de ces ressources n’est pas pris en charge. <!-- GS-3131 -->

* Les utilisateurs doivent se connecter deux fois à un compte Meta Ads de canal lorsqu’ils sont également connectés à Facebook. **Solution** : déconnectez-vous de Facebook avant de vous connecter à un compte de métadonnées de canal.

### Résolution de problèmes connus

* GenStudio affiche une erreur lorsqu’un utilisateur tente de saisir des informations d’identification dans la vue ([!DNL Insights]). (fixe 8/29) <!-- GS-4689 -->

## Versions Beta précédentes

Les versions précédentes de Beta incluaient les mises en évidence et correctifs suivants.

### Tons clairs

* **Score de validation basé sur le pourcentage** : la validation de marque affiche désormais le score de validation de marque sous forme de pourcentage plutôt qu’une valeur de réussite/échec. ([!DNL Brands] 8/16)

* **Interface d’extraction de marque mise à jour** : l’extraction de marque affiche désormais la fin du processus d’extraction sous forme de pourcentage. ([!DNL Brands] 8/16)

* **Chargement incrémentiel de la marque lors de l’extraction** : les directives de marque sont désormais chargées de manière incrémentielle dans l’interface utilisateur. ([!DNL Brands] 8/16)

* **Création d’emails multi-section** : les utilisateurs peuvent désormais créer des emails composés d’éléments distincts pour le titre, l’image, le corps et CTA. ([!DNL Create] 8/16)

* **Redimensionnement des métadonnées publicitaires** : les créateurs peuvent redimensionner les proportions des métadonnées publicitaires. ([!DNL Create] 8/16)

* **Comptes de connexion de statistiques limités** : la connexion de statistiques ne prend désormais en charge qu’un seul compte par client. ([!DNL Insights] 8/16)

### Améliorations supplémentaires et problèmes résolus

* Le nom d’emplacement du flux de page _Détails de l’expérience_ spécifie désormais le flux Facebook ou Instagram. (8/16)

* Le recadrage d’images et de vidéos plus grandes est désormais cohérent lorsque l’utilisateur navigue de la vue _Présentation de la ressource_ vers la vue _Détails de la ressource_. (8/16)

* Le nombre de résultats de recherche sur l’écran Attributs n’affiche plus `0 of` avant qu’un utilisateur ne se connecte.  (8/16) <!-- GS- 3665 -->

* Cliquer sur le champ de comptage **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** n’efface plus les paramètres de recherche et de filtre. (8/16) <!-- GS-3476 -->

### Problèmes connus résolus dans les versions précédentes de Beta

* Le téléchargement des directives sur la marque échoue en raison de problèmes liés à la plateforme de stockage ACP. (fixe 8/22) <!-- GS-4369 -->

* Le menu déroulant Zone d’invite ([!DNL Brands]) affiche un compteur à la fin de la liste ([!DNL Brands]) lors de la création de l’email. (fixe 8/22) <!-- GS-4077 -->

