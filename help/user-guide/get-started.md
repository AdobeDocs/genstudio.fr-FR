---
title: Prise en main de GenStudio
description: Découvrez comment configurer votre GenStudio pour générer un nouveau contenu marketing aligné sur la marque.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 2501d1e36f76d1534a735b9147fb42f762a665e8
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 9%

---


# Prise en main de GenStudio

GenStudio est une plateforme exhaustive qui permet de créer, d’évaluer et de gérer des expériences marketing qui reflètent et adhèrent à votre identité de marque.

L’accès des parties prenantes à ses nombreuses fonctionnalités est contrôlé par des rôles utilisateur attribués. Le rôle d’utilisateur qui vous est attribué détermine les tâches que vous pouvez effectuer dans GenStudio. Un administrateur GenStudio définit vos autorisations, définies dans votre e-mail de bienvenue.

Si vous découvrez les outils génératifs basés sur l’IA ou que vous êtes simplement curieux des principes de base de GenStudio, reportez-vous aux sections [Concepts GenStudio](concepts.md) et [Écrire des invites efficaces](effective-prompts.md).

## Rôles utilisateur GenStudio

La création et le déploiement de campagnes marketing modernes nécessitent une collaboration entre les parties prenantes avec des responsabilités et des compétences variables.

Trois types de rôles utilisateur GenStudio prennent en charge cette diversité de rôles d’organisation. Les autorisations sont adaptées à chacun de ces types d’utilisateurs et prennent en charge les responsabilités de chaque utilisateur au sein de l’organisation marketing.

**Les trois types de rôles utilisateur sont** :

* **Les créateurs** utilisent les fonctionnalités d’IA générative de GenStudio pour créer des ressources de campagne marketing, demander l’approbation et la révision du contenu et publier les brouillons approuvés de ce contenu. Tous les utilisateurs de GensStudio peuvent accéder à une ressource et l’utiliser une fois que son créateur l’a enregistrée dans Contenu.

* **Collaborateurs** sont le plus grand nombre d’utilisateurs de GenStudio. Les collaborateurs peuvent visualiser et approuver le contenu GenStudio. Ils constituent une partie essentielle du workflow, qui garantit que le contenu généré correspond aux exigences et aux normes de votre entreprise.

* **Les administrateurs système** ont le plus grand ensemble d’autorisations dans GenStudio. Les administrateurs système peuvent ajouter et supprimer des utilisateurs et du contenu de Genstudio. Les administrateurs effectuent la tâche essentielle d’intégration consistant à établir les barrières fondamentales pour la création et le déploiement des ressources de campagne. Les administrateurs implémentent ces barrières de sécurité en chargeant des informations spécifiques à la marque et à l’organisation telles que [les directives sur la marque](/help/user-guide/guidelines/overview.md).

>[!NOTE]
>Avant que des utilisateurs ne soient configurés dans ces rôles, un administrateur doit être désigné en tant que superutilisateur dans la console d’administration Adobe pour effectuer les tâches de configuration uniques. Ce rôle de superutilisateur fonctionne uniquement dans le contexte de Adobe Admin Console. Il n’a aucun rôle dans l’interface de la plateforme GenStudio. Il n’existe aucun concept de super-utilisateur dans les affectations de rôles GenStudio.

### Créateurs

**Les créateurs** disposent des autorisations de base nécessaires pour créer des ressources GenStudio [!DNL Brands], [!DNL Campaigns] et [!DNL Content]. Ils peuvent également modifier et supprimer les ressources qu’ils ont créées. GenStudio prend en charge la création rapide de centaines de fragments de contenu. Ces utilisateurs peuvent générer des fragments de contenu ou des expériences complètes qui orchestrent des éléments distincts de contenu approuvé pour répondre aux besoins de campagnes marketing spécifiques.

Les créateurs interagissent avec les technologies d’IA générative GenStudio via _l’invite_. La zone d’invite GenStudio dans la zone de travail fournit des outils pour placer des invites dans le contexte des instructions d’une campagne spécifique. Par conséquent, la qualité et le succès du contenu généré dépendent partiellement de la qualité des directives de marque que votre entreprise a chargées et de la spécificité de votre invite.

Voir [Écrire des invites efficaces](effective-prompts.md).

Le tableau suivant affiche les autorisations de créateur GenStudio par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Mode |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | non | non | non | oui |
| [!DNL Campaigns] | oui | oui | oui | oui |
| [!DNL Content] | oui | oui | oui | oui |
| [!DNL Insights] | peut configurer les connecteurs d’annonces uniquement. |    |     | oui |
| [!DNL Personas] | oui | oui | oui | oui |
| [!DNL Products] | oui | oui | oui | oui |
| [!DNL Reviews and approvals] | oui | oui | oui | oui |

### Collaborateurs

**Les collaborateurs** peuvent afficher des ressources dans GenStudio, mais pas créer, modifier ou supprimer ces ressources. Les collaborateurs incluent les parties prenantes qui sont essentielles au succès du processus de révision et d’approbation du contenu GenStudio, mais qui n’ont pas besoin de créer ou de modifier directement le contenu. Les juristes et les responsables des créateurs sont des exemples de collaborateurs potentiels. Les collaborateurs de GenStudio peuvent disposer des autorisations nécessaires pour créer et afficher des ressources dans d’autres produits de Creative Cloud.

Le tableau suivant affiche les autorisations de collaborateur GenStudio par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Mode |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | oui | oui | oui | oui |
| [!DNL Campaigns] | oui | oui | oui | oui |
| [!DNL Content] | oui | oui | oui | oui |
| [!DNL Insights] | non | non | non | oui |
| [!DNL Personas] | oui | oui | oui | oui |
| [!DNL Products] | oui | oui | oui | oui |
| [!DNL Reviews and approvals] | non | non | non | oui |

### Administrateurs

Les utilisateurs administrateurs créent des utilisateurs et les affectent à l’un des rôles pris en charge par GenStudio. Ils peuvent attribuer de nouvelles autorisations à des créateurs ou collaborateurs individuels, selon les besoins. Leur tâche la plus importante consiste à effectuer les tâches d’intégration initiales qui préparent votre entreprise à déployer GenStudio.

Le tableau suivant affiche les autorisations d’administrateur système GenStudio par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Mode |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | oui | oui | oui | oui |
| [!DNL Campaigns] | oui | oui | oui | oui |
| [!DNL Content] | oui | oui | oui | oui |
| [!DNL Insights] | oui | oui | oui | oui |
| [!DNL Personas] | oui | oui | oui | oui |
| [!DNL Products] | oui | oui | oui | oui |
| [!DNL Reviews and approvals] | oui | oui | oui | oui |


## Préparation de GenStudio pour la génération de contenu

Les administrateurs système préparent l’environnement GenStudio de leur entreprise pour que les créateurs et les collaborateurs puissent créer des ressources de campagne. Ces tâches préliminaires de configuration incluent :

1. [Configurez les instructions](./guidelines/overview.md) pour [!DNL Brands], [!DNL Products] et [!DNL Personas]. Configuration des blocs de création clés de la mar **[Ajoutez des instructions](./guidelines/overview.md)** ([!DNL Brands], [!DNL Products] et [!DNL Personas]) à GenStudio. La configuration des éléments essentiels de l’identité de marque de votre entreprise est une condition préalable essentielle au travail des créateurs et collaborateurs de GenStudio. Vous pouvez charger des documents de directives de marque ou saisir manuellement des informations sur la marque.
   * **Préparez vos documents directives**. Plus vos directives de marque sont descriptives et complètes, plus GenStudio est performant. Incluez de brefs exemples de fonctionnalités que vous considérez comme essentielles pour votre marque et ajoutez des descriptions de comportement que vous souhaitez exclure de la création de contenu GenStudio. GenStudio extrait les informations de ces documents téléchargés et commence à créer votre marque. Les informations telles que les directives sur la voix, le canal et l’image de la marque sont renseignées lorsque GenStudio assemble chaque consigne à partir des documents chargés.
   * **Modifiez ou remplissez les champs de directives de marque selon les besoins**. Des directives de marque complètes constituent la base de la compréhension GenStudio de la marque de votre entreprise. Une fois que GenStudio a extrait les informations dont il a besoin de vos documents d’orientation de marque, vous êtes invité à modifier manuellement ou à compléter les champs des informations extraites. Spécifiez les zones de ciblage de produit individuelles pour la création de contenu en ajoutant un [!DNL Product]. [!DNL Personas] Ces conseils aident à personnaliser la création de contenu pour les segments de clients définis.

   Bien que la configuration des consignes de marque d’une entreprise puisse être une action unique, vous devrez peut-être réviser et améliorer ces consignes en fonction de la volatilité, de la croissance et de l’évolution des circonstances du marché de votre entreprise.

1. **[Télécharger des modèles](./content/use-templates.md)**. Les modèles fournissent des raccourcis et accélèrent la création de contenu. Un modèle contient des fonctionnalités approuvées, telles que des en-têtes et des pieds de page, et établit des barrières de sécurité pour la création de contenu. En règle générale, les administrateurs chargent et gèrent des modèles pour leur entreprise. Les créateurs utilisent des modèles pour lancer le processus de création de contenu dans les limites établies de la marque organisationnelle.

1. **[Télécharger les ressources approuvées](./content/manage-assets.md)**. Les ressources approuvées dans GenStudio [!DNL Content] sont disponibles pour tous les créateurs GenStudio. Vous pouvez créer [!DNL Content] avec des ressources que les créateurs peuvent utiliser pour créer des expériences ou des ressources.

1. **[Connectez-vous à un compte Meta (Facebook)](./insights/connect-channel.md)**. Vous devez configurer une connexion entre GenStudio et les comptes sociaux de votre entreprise pour recevoir les données de vos campagnes marketing, ressources et expériences actives. GenStudio [Insights](./insights/overview.md) fournit des outils pour analyser les données dérivées du canal.
