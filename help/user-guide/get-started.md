---
title: Prise en main de Adobe GenStudio pour les marketeurs de performance
description: Découvrez comment configurer GenStudio pour les marketeurs de performance afin de générer du contenu marketing aligné sur la marque.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: dab19da0063d6f4f4497112c4063bfc9c285e651
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 8%

---

# Prise en main de Adobe GenStudio pour les marketeurs de performance

GenStudio pour les spécialistes du marketing des performances est une plateforme complète permettant de créer, d’évaluer et de gérer des expériences marketing qui reflètent et adhèrent à votre identité de marque.

L’accès des parties prenantes à ses nombreuses fonctionnalités est contrôlé par des _rôles utilisateur_ attribués. Votre rôle d’utilisateur attribué détermine les tâches que vous pouvez effectuer dans GenStudio pour les marketeurs de performances. Un administrateur système Adobe attribue vos autorisations dans le profil de produit GenStudio for Performance Marketing de Adobe Admin Console. Votre e-mail de bienvenue identifie votre rôle attribué.

Si vous découvrez les outils génératifs basés sur l’IA ou que vous êtes simplement curieux des principes de base de GenStudio pour les marketeurs de performances, reportez-vous aux sections [Concepts](concepts.md) et [Écrire des invites efficaces](effective-prompts.md).

## Rôles d’utilisateur ou d’utilisatrice

La création et le déploiement de campagnes marketing modernes nécessitent une collaboration entre les parties prenantes avec des responsabilités et des compétences variables.

Trois types de rôles d’utilisateur GenStudio pour les marketeurs de performance prennent en charge cette diversité de rôles d’organisation. Les autorisations sont adaptées à chacun de ces types d’utilisateurs et prennent en charge les responsabilités de chaque utilisateur au sein de l’organisation marketing.

**Les trois types de rôles utilisateur sont** :

* Les **éditeurs** utilisent GenStudio pour les fonctionnalités d’IA générative des marketeurs de performances afin de créer des ressources de campagne marketing, de demander l’approbation et la révision du contenu et de publier les brouillons approuvés de ce contenu. Tous les utilisateurs de GenStudio peuvent accéder à une ressource et l’utiliser une fois que son créateur l’a enregistrée dans Contenu.

* **Collaborateurs** sont le plus large éventail d’utilisateurs de GenStudio pour les spécialistes du marketing de performances. Les collaborateurs peuvent visualiser et approuver le contenu. Ils constituent une partie essentielle du workflow, qui permet de s’assurer que le contenu que vous générez correspond aux exigences et aux normes de votre entreprise.

* **Les** gestionnaires de système disposent du jeu d’autorisations le plus large dans GenStudio pour les marketeurs de performance. Les gestionnaires de système effectuent la tâche essentielle d’intégration pour établir les barrières de sécurité fondamentales pour la création et le déploiement des ressources de campagne. Les gestionnaires système implémentent ces barrières de sécurité en chargeant des informations spécifiques à la marque et à l’entreprise, telles que les [directives sur la marque](/help/user-guide/guidelines/overview.md). Les gestionnaires de système GenStudio sont autorisés à créer et publier des marques, mais ne disposent pas des privilèges d’administration des utilisateurs.

>[!NOTE]
>Avant que des utilisateurs ne soient configurés dans ces rôles, un administrateur système Adobe doit être désigné dans Adobe Admin Console pour effectuer des tâches de configuration uniques. Ce rôle d’administrateur d’Adobe fonctionne uniquement dans le contexte de Adobe Admin Console. Il n’a aucun rôle dans l’interface de la plateforme GenStudio for Performance Marketing.

### Éditeurs GenStudio

**Les éditeurs** disposent des autorisations de base nécessaires pour créer GenStudio pour les ressources [!DNL Brands], [!DNL Campaigns] et [!DNL Content] des marketeurs de performances. Ils peuvent également modifier et supprimer les ressources qu’ils ont créées. GenStudio pour les spécialistes du marketing des performances prend en charge la création rapide de centaines de fragments de contenu. Ces utilisateurs peuvent générer des sections de contenu ou des expériences complètes qui orchestrent des éléments distincts de contenu approuvé pour répondre aux besoins de campagnes marketing spécifiques.

Les éditeurs interagissent avec GenStudio pour les technologies d’IA générative des marketeurs de performance via _invite_. La zone d’invite de la zone de travail fournit des outils pour placer des invites dans le contexte des instructions d’une campagne spécifique. Par conséquent, la qualité et le succès du contenu généré dépendent partiellement de la qualité des directives de marque que votre entreprise a chargées et de la spécificité de votre invite.

Voir [Écrire des invites efficaces](effective-prompts.md).

Le tableau suivant affiche les autorisations de l’éditeur par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Afficher |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | non | non | non | oui |
| [!DNL Campaigns] | oui | oui | oui | oui |
| [!DNL Content] | oui | oui | oui | oui |
| [!DNL Insights] | peut configurer les connecteurs d’annonces uniquement. |    |     | oui |
| [!DNL Personas] | oui | oui | oui | oui |
| [!DNL Products] | oui | oui | oui | oui |
| [!DNL Reviews and approvals] | oui | oui | oui | oui |

### Collaborateurs GenStudio

**Les collaborateurs** peuvent afficher des ressources dans GenStudio pour les marketeurs de performance, mais pas créer, modifier ou supprimer ces ressources. Les collaborateurs incluent les parties prenantes qui sont essentielles au succès du processus de révision et d’approbation du contenu, mais qui n’ont pas besoin de créer ou de modifier directement le contenu. Les juristes et les responsables des créateurs sont des exemples de collaborateurs potentiels. Les collaborateurs GenStudio pour les marketeurs de performance peuvent disposer des autorisations nécessaires pour créer et afficher des ressources dans d’autres produits Creative Cloud.

Le tableau suivant affiche les autorisations de collaborateur par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Afficher |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | non | non | non | oui |
| [!DNL Campaigns] | non | non | non | oui |
| [!DNL Content] | non | non | non | oui |
| [!DNL Insights] | non | non | non | oui |
| [!DNL Personas] | non | non | non | oui |
| [!DNL Products] | non | non | non | oui |
| [!DNL Reviews and approvals] | non | non | non | oui |

### Gestionnaire de système GenStudio

**Les gestionnaires de système GenStudio** effectuent les tâches initiales qui préparent votre entreprise à déployer GenStudio pour les marketeurs de performance.

Le tableau suivant affiche les autorisations par défaut du gestionnaire de système GenStudio :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Afficher |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | oui | oui | oui | oui |
| [!DNL Campaigns] | oui | oui | oui | oui |
| [!DNL Content] | oui | oui | oui | oui |
| [!DNL Insights] | oui | oui | oui | oui |
| [!DNL Personas] | oui | oui | oui | oui |
| [!DNL Products] | oui | oui | oui | oui |
| [!DNL Reviews and approvals] | oui | oui | oui | oui |


## Préparation de GenStudio pour la génération de contenu par les marketeurs de performance

Les gestionnaires de système GenStudio préparent l’environnement GenStudio pour les marketeurs de performance de leur entreprise afin que les éditeurs et les collaborateurs puissent créer des ressources de campagne. Ces tâches préliminaires de configuration incluent :

1. [Ajoutez des instructions](./guidelines/overview.md) pour [!DNL Brands], [!DNL Products] et [!DNL Personas]. La configuration des éléments essentiels de l’identité de marque de votre entreprise est une condition préalable essentielle au travail des créateurs et des collaborateurs. Vous pouvez charger des documents de directives de marque ou saisir manuellement des informations sur la marque.
   * **Préparez vos documents directives**. Plus vos directives de marque sont descriptives et complètes, plus la sortie est bonne. Incluez de brefs exemples de fonctionnalités que vous considérez essentielles à votre marque et ajoutez des descriptions de comportement que vous souhaitez exclure de la création de contenu. GenStudio for Performance Marketing extrait des informations de ces documents téléchargés et commence à créer votre marque. Les informations telles que les directives sur la voix, le canal et l’image de la marque sont renseignées lorsque GenStudio pour les spécialistes du marketing des performances rassemble chaque consigne à partir des documents chargés.
   * **Modifiez ou remplissez les champs de directives de marque selon les besoins**. Des directives complètes sur la marque constituent la base de la compréhension de la marque par les marketeurs des performances de GenStudio. Une fois que GenStudio for Performance Marketing a extrait les informations dont il a besoin de vos documents de directives de marque, vous êtes invité à modifier manuellement ou à compléter les champs d’informations extraites. Spécifiez les zones de ciblage de produit individuelles pour la création de contenu en ajoutant un [!DNL Product]. [!DNL Personas] Ces conseils aident à personnaliser la création de contenu pour les segments de clients définis.

   Bien que la configuration des consignes de marque d’une entreprise puisse être une action unique, vous devrez peut-être réviser et améliorer ces consignes en fonction de la volatilité, de la croissance et de l’évolution des circonstances du marché de votre entreprise.

1. **[Télécharger des modèles](./content/use-templates.md)**. Les modèles fournissent des raccourcis et accélèrent la création de contenu. Un modèle contient des fonctionnalités approuvées, telles que des en-têtes et des pieds de page, et établit des barrières de sécurité pour la création de contenu. En règle générale, les gestionnaires système chargent et gèrent des modèles pour leur entreprise. Les créateurs utilisent des modèles pour lancer le processus de création de contenu dans les limites établies de la marque organisationnelle.

1. **[Télécharger les ressources approuvées](./content/manage-assets.md)**. Les ressources approuvées dans [!DNL Content] sont disponibles pour tous les créateurs GenStudio pour les marketeurs de performances. Vous pouvez créer [!DNL Content] avec des ressources que les créateurs peuvent utiliser pour créer des expériences ou des ressources.

1. **[Connectez-vous à un compte Meta (Facebook)](./insights/connect-channel.md)**. Configurez une connexion entre GenStudio pour les spécialistes du marketing des performances et les comptes sociaux de votre entreprise afin de recevoir les données de vos campagnes marketing, ressources et expériences actives. [[!DNL Insights]](./insights/overview.md) fournit des outils pour analyser les données dérivées du canal.
