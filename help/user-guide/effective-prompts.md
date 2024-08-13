---
title: Écrire les invites efficaces
description: Découvrez comment écrire des invites efficaces pour GenStudio.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
source-git-commit: 5e17996ee3a86cf664ee468d6b9cf178c8853992
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Écrire les invites efficaces

La communication avec l’IA générative est essentielle pour travailler efficacement dans GenStudio.

GenStudio fournit une invite d’IA générative chaque fois qu’il est possible de modifier une ressource. Les composants d’une invite efficace doivent inclure un langage descriptif, des exemples et des informations qui ne sont pas fournis par le biais de vos instructions configurées.

En règle générale, fournissez à GenStudio des informations sur votre marque en utilisant [des instructions](/help/user-guide/guidelines/overview.md), puis vous pouvez exploiter pleinement l’IA générative pour produire des expériences de contenu alignées sur la marque.

## Langage descriptif

Vous pouvez utiliser un langage naturel pour articuler vos idées pour créer des expériences. Votre invite guide l’IA pour générer du contenu de canal personnalisé et des images qui complètent votre vision. Plus vous fournissez de détails, plus grande est la probabilité de produire une image ou une expérience qui répond à vos besoins. Utilisez un langage clair et descriptif afin de fournir le plus de détails possible :

- Pour **images**, utilisez des mots qui décrivent l’ambiance, l’humeur, la couleur, la composition et le style.
- Pour **copy**, utilisez des mots qui décrivent l’audience, l’objectif, les nouvelles descriptions de fonctionnalités, les exemples et les actions.

Vous trouverez ci-dessous un exemple d’invite qui fournit des informations sur votre intention, votre audience cible et votre style.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Voir les exemples de résultats

![trois emails générés](/help/assets/sample-email.png)

+++

## Critères d’invite

Dans GenStudio [[!DNL Create]](/help/user-guide/create/overview.md), vous pouvez utiliser les **[!UICONTROL critères d’invite]** ([_Paramètres_](/help/user-guide/create/overview.md#parameters) et une invite) dans la zone d’invite pour ajouter des détails par le biais de la sélection afin d’améliorer l’interprétation de l’IA.

Pour [emails](/help/tutorials/create-email-experience.md), les critères d’invite peuvent inclure l’ajout de [guidelines](/help/user-guide/guidelines/overview.md) dans _Parameters_, le chargement d’une ressource à utiliser dans les variantes d’email et une invite descriptive. Pour une [méta-publicité](/help/tutorials/create-meta-ad.md), les critères d’invite peuvent inclure une ligne directrice de la marque dans _Paramètres_, la sélection ou le chargement d’une ressource existante, des paramètres liés aux images ou aux ressources tels que les proportions et une invite. La puissance réelle commence par [la configuration des instructions GenStudio](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Si des instructions sont ajoutées dans la zone d’invite _Parameters_ , il n’est pas nécessaire d’inclure des références à celles de votre invite. GenStudio exploitera ces [!DNL Brands], [!DNL Products] et [!DNL Personas] lors de la génération du contenu.

### Instructions

Les instructions de GenStudio aident l’IA générative à personnaliser la composition de vos ressources GenStudio. Lorsque des critères d’invite s’affichent, vous pouvez choisir un [[!DNL Brand]](/help/user-guide/guidelines/brands.md), un [[!DNL Persona]](/help/user-guide/guidelines/personas.md) et un [[!DNL Product]](/help/user-guide/guidelines/products.md) parmi les instructions que vous avez configurées.

>[!TIP]
>
>Vous contrôlez comment et quand GenStudio utilise vos instructions [!DNL Brand]. Voir [Instructions](/help/user-guide/guidelines/overview.md) pour savoir comment configurer et gérer les directives de votre marque.

## Réessayer

Prompter est un processus itératif. Si les résultats ne répondent pas à vos attentes, passez en revue votre invite et apportez des modifications ou ajoutez des détails supplémentaires. Vous pouvez affiner votre invite en fournissant une URL comme exemple ou une source pour plus d’informations.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.

Use information from https://www.adobe.com/products/photoshop.html to inspire users with the latest features.
```

Vous pouvez également coller des sections dans un résumé de campagne. Vous pouvez même demander à GenStudio d’éviter certains mots, éléments ou thèmes.

## Bonnes pratiques

Quelques bonnes pratiques simples pour créer des invites efficaces dans GenStudio :

- Soyez précis et fournissez des détails sur ce qu’il faut faire ou non.
- Fournir du contexte à l’aide de références externes.
- Appliquez les directives de GenStudio.
- Examinez et ajustez régulièrement les consignes.
- Itérer et affiner.
- Apprenez par l&#39;expérimentation.
