---
title: Détails de la ressource
description: GenStudio stocke le contenu approuvé avec des métadonnées enrichies pour le suivi de la recherche et des performances.
feature: Attributes, Assets
source-git-commit: ba7dced9e62f797cd43a0bd8d8263828ec5c3d5e
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 7%

---


# Détails de la ressource

GenStudio stocke le contenu approuvé avec des métadonnées enrichies pour le suivi des performances et de la capacité de découverte.

Chaque ressource (y compris les expériences et les modèles) est associée à _details_ (métadonnées) qui permettent d’identifier, de suivre, d’utiliser et d’apprendre des performances du contenu.

Les types de métadonnées de ressources incluent [les métadonnées système](#system-metadata) et [ les métadonnées définies par l’utilisateur](#user-defined-metadata).

## Métadonnées système

Certaines métadonnées de ressource sont automatiquement collectées lorsqu’une ressource est chargée. Vous ne pouvez pas modifier les métadonnées système par défaut.

Les métadonnées par défaut stockées et capturées pour une ressource incluent le nom, les dimensions, la source, etc. du fichier.

### Balises générées

Lorsque les ressources sont approuvées et stockées dans [!DNL Content], GenStudio utilise les fonctionnalités d’intelligence artificielle et d’apprentissage automatique d’Adobe pour générer des balises en fonction des fonctionnalités de la ressource, telles que la couleur et le ton, ou les mots-clés qui identifient les fonctionnalités de la ressource. Vous ne pouvez pas modifier de balises.

### Métadonnées de contenu générées

Les informations utilisées pour générer une nouvelle ressource ou expérience deviennent des métadonnées, telles que l’invite qui a été utilisée. Vous ne pouvez pas modifier l’invite une fois le contenu validé, mais vous pouvez l’utiliser comme point de départ pour générer quelque chose de nouveau.

## Métadonnées définies par les utilisateurs

Les métadonnées définies par l’utilisateur ajoutent du contexte marketing au contenu de la ressource, ce qui permet aux marketeurs de mieux comprendre comment utiliser la ressource et interagir avec elle.

Lorsque vous [téléchargez une ressource](/help/user-guide/content/manage-assets.md#add-assets), vous pouvez définir un ensemble de détails de ressource facultatifs qui existent dans GenStudio en tant que métadonnées.

### Détails des métadonnées

Le tableau suivant détaille les métadonnées (détails de la ressource) que vous pouvez définir lors de la création d’une ressource.

| Champ | Description | Modifiable | Obligatoire |
| ------------- | ----------- | -------- | -------- |
| Nom de la campagne (nom du projet) | Métadonnées par défaut capturées et stockées avec la ressource | Y | N |
| Nom de la marque | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) ajouté à GenStudio et publié pour utilisation | Y | N |
| Produits | [[!DNL Products]](/help/user-guide/guidelines/products.md) ajouté à GenStudio pour utilisation | Y | N |
| Personnes | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) ajouté à GenStudio pour utilisation | Y | N |
| Canaux | Types de contenu dans GenStudio pour lesquels la ressource est utilisée, tels que les courriers électroniques et les métadonnées publicitaires | Y | N |
| Période | Période pour laquelle la ressource a été utilisée, par exemple trimestre, saison, année, etc. Exemple : `Winter 2023` | Y | N |
| Région   | Régions pour lesquelles la ressource est utilisée. Exemples : `North America`, `APAC`, `Italy` | Y | N |
| Langue | Langues pour lesquelles la ressource est utilisée. Exemple : `Spanish` | Y | N |
| Mots-clés | Mots-clés utilisés pour identifier l’objectif de la ressource | Y | N |

## Affichage des détails de la ressource

**Pour afficher les détails de la ressource** :

1. Dans _[!DNL Content]_, sélectionnez une ressource.

1. Dans la vue de la ressource, passez en revue la section _[!UICONTROL Details]_ à droite.

   Si la section _[!UICONTROL Détails]_ n&#39;est pas visible, cliquez sur l&#39;icône **[!UICONTROL Informations]** (i).

>[!TIP]
>
>Vous pouvez également afficher les détails des ressources à partir de [!DNL Insights]. Insights fournit des statistiques d’utilisation et un contexte de performances entre les expériences. Dans _[!DNL Insights]_, sélectionnez la section **[!UICONTROL Assets]**.

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
