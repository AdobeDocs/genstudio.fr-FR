---
title: Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio.
source-git-commit: 382026b07e123a1e49813b766f69496f6a8f38eb
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 2%

---


# Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta

Ces notes mettent en évidence d’importants correctifs d’Adobe GenStudio et améliorations pour la semaine se terminant le 16 août.

## Tons clairs

Le développement des fonctionnalités de GenStudio est rapide et continu. Les nouvelles fonctionnalités notables sont les suivantes :

### Marque

Le panneau de validation de marque a été amélioré afin d’améliorer l’expérience utilisateur, notamment les modifications suivantes :

* _Score de validation basé sur le pourcentage_ : la validation de marque affiche désormais le score de validation de marque sous forme de pourcentage plutôt qu’une valeur de réussite/échec.

* _Interface d’extraction de marque mise à jour_ : l’extraction de marque affiche désormais la fin du processus d’extraction sous forme de pourcentage.

* _Chargement incrémentiel de la marque lors de l’extraction_ : les directives de marque sont désormais chargées de manière incrémentielle dans l’interface utilisateur.

* _Simplification du schéma de ligne guide de copie_ : les champs `unique attributes` et `frequent keywords` ont été supprimés du schéma de ligne guide de copie, ce qui simplifie le processus de configuration de ligne guide.

* _Génération d’images : sélection de catégorie_ : les utilisateurs peuvent désormais sélectionner les directives d’image spécifiques à leurs besoins de régénération d’image.

### Créer

* **Création d’emails multi-section** : les utilisateurs peuvent désormais créer des emails composés d’éléments distincts pour le titre, l’image, le corps et CTA.

* **Redimensionnement des métadonnées publicitaires** : les créateurs peuvent redimensionner les proportions des métadonnées publicitaires.

### Insights

* **Comptes de connexion de statistiques limités** : la connexion de statistiques ne prend désormais en charge qu’un seul compte par client.

## Améliorations et problèmes résolus

Cette version comprend les correctifs supplémentaires suivants.

### Insights

* Le nom d’emplacement du flux de page _Détails de l’expérience_ spécifie désormais le flux Facebook ou Instagram.

* Le recadrage d’images et de vidéos plus grandes est désormais cohérent lorsque l’utilisateur navigue de la vue _Présentation de la ressource_ vers la vue _Détails de la ressource_.

* Le nombre de résultats de recherche sur l’écran Attributs n’affiche plus `0 of` avant qu’un utilisateur ne se connecte. <!-- GS- 3665 -->

* Cliquer sur le champ de comptage **[!UICONTROL Insight]** > **[!UICONTROL Asset]** n’efface plus les paramètres de recherche et de filtre. <!-- GS-3476 -->

## Problèmes connus

Les problèmes connus suivants seront résolus par la version GA de GenStudio pour les marketeurs de performance.

### Analytique

* Les actions déclenchées par les boutons **[!UICONTROL Ajouter des modèles]** et **[!UICONTROL Télécharger]** ne sont actuellement pas suivies. <!-- GS-3505 -->

### Marque

* Un créateur peut publier une marque, mais les membres de l’organisation ne peuvent pas la voir. <!-- XI-2197 -->

### Créer

* Le recadrage des images dans les métadonnées publicitaires est incohérent. <!-- GS-3739 -->

* Les modèles composés de plusieurs groupes d’éléments de page échouent à la validation de la marque. <!-- GS-4037 -->

### Insights

* Les erreurs d’accès refusé se produisent avec le point de terminaison `/admin/addOffer` (service de mise en service). **Résolu 8/12**. <!-- GS-4047 -->

* Les valeurs **Dépensé au niveau de la campagne** ne sont pas exactes. Actuellement, les données ne sont pas cohérentes entre Facebook Ads Manager et le lac de données. <!-- GS-3202 -->

### Révisions et approbations

* Les créateurs peuvent modifier les ressources après approbation avant de les publier. Les approbateurs ne sont pas informés de ces modifications.
