---
title: Adobe GenStudio pour les révisions et approbations des marketeurs de performance
description: Découvrez le processus de révision et d’approbation de GenStudio for Performance Marketing.
feature: Approval
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Adobe GenStudio pour les révisions et approbations des marketeurs de performance

Le workflow d’examen et d’approbation de GenStudio pour les marketeurs de performance garantit que toutes les parties prenantes, des équipes créatives aux experts juridiques, peuvent examiner et approuver efficacement les composants de campagne, y compris les ressources de marque générées par l’IA.

## Avantages du workflow [!DNL Review and Approval]

* **Prise en charge de la création de contenu d’IA itérative et robuste**. La création et le déploiement de contenu aligné sur la marque dans une entreprise est un processus hautement itératif. Les fonctionnalités d’IA générative de GenStudio for Performance Marketing prennent en charge la création rapide de centaines de variantes de ressources. Chaque réviseur peut demander plusieurs modifications à un brouillon de ressource avant de l’approuver. Plus les réviseurs sont nombreux, plus le nombre d&#39;itérations potentielles est élevé avant que toutes les parties prenantes ne s&#39;accordent sur une variante finale.

* **Prise en charge de l’intégrité créative**. Les approbations protègent l’intégrité créative des ressources de marque en maintenant les créateurs de contenu impliqués dans le processus d’approbation. En impliquant les parties prenantes créatives (par exemple, les créateurs de contenu et les directeurs créatifs) dans le processus de révision et d’approbation, vous vous assurez que la sortie finale s’aligne sur votre vision et votre identité de marque.

* **Respect des objectifs de Campaign et des exigences légales**. Le processus d’approbation permet de vérifier que le contenu prend en charge les objectifs de la campagne. Il garantit que le contenu respecte l’authenticité juridique, ce qui minimise les risques et les problèmes juridiques potentiels.

## Cycle de vie de révision et d’approbation

Les phases principales du workflow de révision et d’approbation sont les suivantes :

* [Demander la révision et l’approbation du contenu que vous avez créé](./request-review.md)
* [Révision et modification du contenu](./review-and-edit.md)
* [Valider le contenu](./approve-content.md)
* [Contenu Publish](./publish-content.md)

## Qui peut demander une révision ou approuver un contenu ?

Si vous avez créé une ressource ou une expérience, vous pouvez demander à d’autres personnes de la chaîne d’approbation de votre organisation de passer en revue et de commenter officiellement votre travail. Seuls ces approbateurs désignés peuvent examiner le brouillon.

## À propos de [!DNL Content] brouillons

_Les brouillons_ sont des versions préliminaires de ressources ou d’expériences qui n’ont pas subi le processus de révision et d’approbation. L’état Version préliminaire identifie l’emplacement du brouillon dans le processus de révision et d’approbation. Un ID de brouillon unique identifie chaque brouillon. L’ID est valide jusqu’à ce qu’un brouillon soit approuvé et publié sur [!DNL Content]. Les commentaires de révision et les approbations pour un brouillon sont associés à cet ID de brouillon individuel.

Lorsqu’un brouillon termine le processus de révision et d’approbation et est publié sur [!DNL Content], l’ID de brouillon expire et GenStudio pour les marketeurs de performances n’enregistre pas les commentaires et les états d’approbation associés. L’URL du brouillon n’est plus valide.

L’état Version préliminaire capture l’état du brouillon de contenu au fur et à mesure qu’il passe par le processus de révision et d’approbation. Tous les réviseurs désignés sont informés des modifications de l’état du contenu qu’ils sont en train de vérifier. Les réviseurs modifient l’état du brouillon pour indiquer si un brouillon doit être révisé plus avant ou s’il peut être approuvé. Tous les approbateurs désignés doivent approuver une ressource ou une expérience avant qu’elle ne puisse être publiée.

Statuts de brouillon disponibles :

**Notifié** : le créateur de contenu a démarré le processus de révision en informant les réviseurs qu’un brouillon est prêt pour la révision.
**Travail nécessaire** : indique qu’un ou plusieurs réviseurs ont demandé des modifications au brouillon de contenu. Le contenu de cet état ne peut pas être enregistré dans [!DNL Content].
**Approuvé** : tous les approbateurs désignés ont approuvé la ressource ou l’expérience. Le créateur de contenu peut maintenant ajouter des métadonnées à la ressource ou à l’expérience et les enregistrer dans [!DNL Content].

## Notifications

Les notifications internes à GenStudio for Performance Marketers mettent à jour les approbateurs et les créateurs de contenu en temps réel lors des modifications d’état des ressources et des commentaires de révision. Les notifications prennent en charge l’itération rapide par le biais de plusieurs cycles de révision, de modification et d’approbation.

Les actions entreprises par les participants à l’approbation déclenchent des notifications internes et des notifications électroniques automatiques. Lorsque vous lancez un processus d’approbation, les approbateurs désignés reçoivent des notifications par courrier électronique et des notifications internes au produit. Vous êtes tenu dans la boucle avec des notifications internes au produit chaque fois qu’un approbateur ajoute des commentaires ou approuve. Les notifications comprennent des liens vers le brouillon de contenu.

Si vous avez lancé le processus de révision et d’approbation du contenu, vous êtes informé de toutes les approbations et de tous les commentaires de révision. Cependant, les approbateurs sont avertis uniquement des commentaires qui les incluent avec un `@mention`.
