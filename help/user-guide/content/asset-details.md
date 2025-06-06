---
title: Détails de la ressource
description: Adobe GenStudio for Performance Marketing stocke le contenu approuvé avec des métadonnées enrichies pour le suivi des performances et de la recherche.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: bd3c5c9ff12c962d4123ac992fb74cd94e184172
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 1%

---

# Détails de la ressource

Adobe GenStudio for Performance Marketing stocke le contenu approuvé avec des métadonnées enrichies pour le suivi des performances et de la capacité de découverte.

Chaque ressource (y compris les expériences et les modèles) est associée à _details_ (métadonnées) qui permettent d’identifier, de suivre, d’utiliser et d’apprendre des performances du contenu.

**Pour afficher les détails de la ressource** :

1. Dans _[!DNL Content]_, sélectionnez une ressource, une expérience ou un modèle. Cliquer sur une ressource ouvre une vue sélectionnée de la ressource.

1. Dans la vue de la ressource, passez en revue la section _[!UICONTROL Details]_ à droite.

   >[!TIP]
   >
   >Si la section _[!UICONTROL Détails]_ n&#39;est pas visible, cliquez sur l&#39;icône **[!UICONTROL Informations]** (i).

   Les détails de la ressource incluent les métadonnées appliquées au cours du processus de création ou de chargement. Les types de métadonnées de ressources incluent [les métadonnées système](#system-metadata) et [ les métadonnées définies par l’utilisateur](#user-defined-metadata).

>[!NOTE]
>
>Assets des référentiels AEM affiche différentes métadonnées. Voir [Configuration de la visibilité des ressources](connect-aem-repo.md#step-4-configure-asset-visibility) pour apprendre à configurer les [!DNL AEM Assets Content Hub] détails des ressources.

## Modifier dans Express

Vous pouvez modifier des ressources d’image (JPG ou PNG) directement dans GenStudio for Performance Marketing à l’aide d’Adobe Express. Le canevas _[!UICONTROL Powered by Adobe Express]_ offre des fonctionnalités pratiques pour améliorer vos images sans quitter l’application GenStudio. Vous pouvez facilement supprimer des arrière-plans, appliquer des remplissages génératifs, ajuster les effets et recadrer des images.

1. Dans _[!DNL Content]_, sélectionnez une ressource image. Cliquer sur une ressource ouvre une vue sélectionnée de la ressource.

1. Dans la vue de la ressource, cliquez sur l&#39;icône **[!UICONTROL Modifier en Adobe Express]** en haut à droite.

1. Dans la zone de travail _[!UICONTROL Powered by Adobe Express]_, utilisez les commandes express du panneau de gauche pour améliorer votre image.

1. Lorsque vous êtes satisfait de l’image mise à jour, cliquez sur **[!UICONTROL Enregistrer une copie]** dans le coin supérieur droit.

1. Sélectionnez le format de fichier (JPG ou PNG) et cliquez sur **[!UICONTROL Enregistrer une copie]**.

1. Dans la fenêtre contextuelle _[!UICONTROL Enregistrer une copie de la ressource]_, mettez à jour le **[!UICONTROL nom de la ressource]**.

   - Sélectionnez **[!UICONTROL Même détails que la ressource d’origine]** pour transférer les détails de la ressource vers la nouvelle image.

   - Développez la section **[!UICONTROL Plus de détails]** pour mettre à jour Campaign, les directives et d’autres métadonnées.

   >[!TIP]
   >
   >Plus vous fournissez de détails, plus vous découvrez les puissantes fonctionnalités de GenStudio for Performance Marketing. Sélectionnez un ou plusieurs détails dans la liste ou saisissez-en un nouveau le cas échéant, par exemple avec des mots-clés. Chaque détail que vous ajoutez apparaît sous la liste. Cliquez sur **`x`** pour supprimer un détail.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

## Métadonnées système

Certaines métadonnées de ressource sont automatiquement collectées lorsqu’une ressource est chargée. Vous ne pouvez pas modifier les métadonnées système par défaut.

Les métadonnées par défaut stockées et capturées pour une ressource incluent le nom, les dimensions, la source, etc. du fichier.

### Balises générées

Lorsque vous stockez une ressource approuvée dans [!DNL Content], GenStudio for Performance Marketing utilise les fonctionnalités d’IA et d’apprentissage automatique d’Adobe pour étudier la ressource et appliquer des balises en fonction des fonctionnalités de la ressource. Par exemple, une image d’un chat peut générer des balises d’attribut telles que `pet photography` ou `cat`, ainsi que des balises de couleur qui identifient les couleurs dominantes de l’image. Vous ne pouvez pas modifier de balises.

Voir [Attributs de statistiques](/help/user-guide/insights/attributes.md).

### Métadonnées de contenu générées

Les informations utilisées pour générer une nouvelle ressource ou expérience deviennent des métadonnées, telles que l’invite qui a été utilisée. Vous ne pouvez pas modifier l’invite une fois le contenu validé, mais vous pouvez l’utiliser comme point de départ pour générer quelque chose de nouveau.

## Métadonnées définies par les utilisateurs

Les métadonnées définies par l’utilisateur ajoutent du contexte marketing au contenu de la ressource, ce qui permet aux marketeurs de comprendre comment utiliser la ressource et interagir avec elle.

Lorsque vous [téléchargez une ressource](/help/user-guide/content/manage-assets.md#add-assets), vous pouvez définir un ensemble de détails de ressource facultatifs qui existent dans GenStudio for Performance Marketing en tant que métadonnées. L’inclusion d’autres détails peut améliorer l’identification des ressources dans les recherches et le filtrage.

### Détails des métadonnées

Le tableau suivant décrit les métadonnées (détails de la ressource) que vous pouvez définir lors de la création d’une ressource.

| champ | Description |
| ------------- | ----------- |
| Campagnes (nom du projet) | Métadonnées par défaut capturées et stockées avec la ressource |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) ajouté à GenStudio for Performance Marketing et publié pour utilisation |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) ajouté à GenStudio for Performance Marketing pour utilisation |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) ajouté à GenStudio for Performance Marketing pour utilisation |
| Canaux | Types de contenu dans GenStudio for Performance Marketing pour lesquels la ressource est utilisée, tels que les courriers électroniques et les métadonnées publicitaires |
| Période | Période pour laquelle la ressource a été utilisée, par exemple trimestre, saison, année, etc. Exemple : `Winter 2023` |
| Région   | Régions pour lesquelles la ressource est utilisée. Exemples : `North America`, `APAC`, `Italy` |
| Langue | Langues pour lesquelles la ressource est utilisée. Exemple : `Spanish` |
| Mots-clés | Mots-clés utilisés pour une identification plus approfondie des caractéristiques et de l’objectif des ressources |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
