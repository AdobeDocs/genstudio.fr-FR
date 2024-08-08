---
title: Préparation d’un modèle de courrier électronique pour GenStudio
description: Découvrez comment créer un modèle de courrier électronique personnalisé pour GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 6870f1b7056219d03cabbcc4e5ddbfa436b1a56d
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Préparer le modèle de courrier électronique pour GenStudio

En règle générale, un concepteur crée la conception visuelle d’un modèle dans un programme de conception tel qu’Adobe XD. Une fois qu’un modèle d’email a été conçu, codé et testé, vous pouvez le préparer pour le chargement et l’utilisation dans GenStudio.

Voir [Anatomie d’un modèle](/help/user-guide/content/use-templates.md#anatomy-of-a-template).

## Ajouter des instructions

Avant de préparer un modèle de métadonnées publicitaires, assurez-vous d’avoir ajouté [des instructions](/help/user-guide/guidelines/overview.md) à votre GenStudio et de leur avoir fourni des informations complètes sur les marques pertinentes. Les [directives de marque](/help/user-guide/guidelines/brands.md) influent directement sur le contenu généré.

> **Exemple** : si vous souhaitez que le corps d’un modèle de courrier électronique ne dépasse pas 500 caractères, ajoutez cette exigence au [guide du canal](/help/user-guide/guidelines/brands.md#channel-guidelines) pour le champ &quot;body&quot;.

## Code un modèle de courrier électronique

Une fois le modèle conçu, il est codé à l’aide d’HTML et de CSS intégré. Le code doit être propre et réactif pour divers appareils.

Voir [Exemples de modèles](/help/user-guide/content/customize-template.md#template-examples).

## Tester un modèle d&#39;email

Utilisez votre diffusion email ou votre plateforme de vérification pour tester votre email et vérifier qu’il s’affiche correctement sur différents clients et appareils de messagerie.

Testez pour vous assurer que votre modèle d&#39;email répond aux critères suivants :

* La mise en page s’ajuste pour différentes tailles d’écran à l’aide de requêtes multimédias CSS
* Vous pouvez cliquer sur les boutons et accéder à l’emplacement prévu
* Le modèle d’email est lisible et utilisable sur les appareils mobiles

## Définition des zones de contenu générées

Définissez les zones de votre modèle de courrier électronique qui doivent être renseignées dynamiquement avec le contenu de GenStudio.

Pour définir les zones de contenu générées :

* Identifiez les éléments de texte dans le modèle que GenStudio doit générer automatiquement, tels que le titre ou CTA.
* Adaptez votre modèle d’HTML en y insérant des espaces réservés à l’aide de la syntaxe Handblebars .

Voir [Espaces réservés de contenu](/help/user-guide/content/customize-template.md#content-placeholders).

## Prévisualiser le modèle

Contrôlez la visibilité de zones de contenu spécifiques à l’aide des assistants intégrés. Par exemple, vous pouvez inclure des paramètres de suivi aux liens dans un modèle exporté tout en conservant des liens d’aperçu propres.

Voir [Aperçu du modèle](/help/user-guide/content/customize-template.md#template-preview).

## Télécharger et utiliser un modèle

Une fois votre modèle conçu, codé, testé et prévisualisé, vous pouvez le charger dans GenStudio afin de l’utiliser pour générer du nouveau contenu marketing.

Voir [Utilisation de modèles](use-templates.md).