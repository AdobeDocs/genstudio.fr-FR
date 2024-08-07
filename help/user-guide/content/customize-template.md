---
title: Personnalisation des modèles
description: Découvrez comment créer un modèle personnalisé pour GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 423956d6fdbf5b31041d44eb434f90d55a87d7c0
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---


# Personnalisation des modèles

Vous pouvez adapter vos modèles d’HTML pour GenStudio en utilisant le langage de modèle _Handlebars_. La syntaxe Handlebars utilise du texte normal avec des accolades doubles comme espaces réservés au contenu. Voir [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) dans le _guide de langue Handlebars_ pour apprendre à préparer votre modèle.

## Structure du modèle

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->

Si vous ne disposez pas d’un modèle d’HTML prêt à l’emploi dans GenStudio, vous pouvez commencer par définir la structure de votre email à l’aide des balises d’HTML : `DOCTYPE`, `html`, `head` et `body`. Vous pouvez inclure des styles CSS pour personnaliser l’aspect de votre email.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Title</title>
    <style>
    </style>
</head>
<body>
</body>
</html>
```

>[!TIP]
>
>Dans les sections suivantes, ajoutez des espaces réservés de contenu aux champs d’email, masquez les éléments superflus de l’aperçu et gérez les liens vers du contenu statique. Une fois votre modèle prêt, vous pouvez [le charger vers GenStudio](use-templates.md#upload-a-template) et commencer à générer des emails personnalisés basés sur votre modèle personnalisé.

## Espaces réservés de contenu

Dans l’en-tête ou dans le corps du modèle, vous pouvez utiliser la syntaxe Handlebars pour insérer des espaces réservés de contenu dans lesquels vous avez besoin de GenStudio pour remplir l’email avec du contenu réel. GenStudio reconnaît et interprète automatiquement les espaces réservés de contenu en fonction du nom du champ.

Par exemple, vous pouvez utiliser `{{ headline }}` pour indiquer où le titre de l&#39;email doit être placé :

```handlebars
<div>{{ headline }}</div>
```

Le nombre maximal de champs autorisés dans un modèle personnalisé est de vingt.

**Noms de champ reconnus** :

| Champ | Rôle | Modèle de canal |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | En-tête pre | email |
| `headline` | Titre | email<br>publicité sociale |
| `body` | Copie de contenu | email<br>publicité sociale |
| `cta` | Appel à l’action | email<br>publicité sociale |
| `on_image_text` | Sur le texte de l’image | publicité sociale |
| `image` | Image | email<br>publicité sociale |
| `brand_logo` | Logo de la marque sélectionnée | publicité sociale |

>[!IMPORTANT]
>
>GenStudio fournit automatiquement le modèle de courrier électronique avec un champ `subject` pendant le processus [!DNL Create]. Il n’est donc pas nécessaire d’inclure l’objet dans votre modèle de courrier électronique.

+++Exemple : modèle de base

Voici un exemple de base d’un modèle d’HTML pour un email. L’en-tête contient une feuille CSS simple et intégrée pour la mise en forme. Le corps contient un espace réservé `pre-header`, `headline` et `image` à utiliser par GenStudio pour injecter du contenu pendant le processus de génération de courrier électronique.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

### Image d’arrière-plan

Lors de la conception d’une publicité pour les métadonnées, il est important d’utiliser une image d’arrière-plan complétée par du texte et une superposition de logo de marque. Pour garantir une mise à l’échelle correcte de l’image, les modèles de métadonnées publicitaires nécessitent la spécification d’un `aspect ratio`. Dans ce contexte, vous ne pouvez fournir qu’un seul champ d’image.

## Sections ou groupes

_Les sections_ permettent d’informer GenStudio que les champs appartenant à une section nécessitent un haut degré de cohérence. L’établissement de cette relation permet à l’IA de générer du contenu correspondant aux éléments créatifs de la section . Un modèle peut comporter trois sections au maximum.

Utilisez un préfixe de votre choix dans le nom du champ pour indiquer que ce champ fait partie d’une section ou d’un groupe. Par exemple, vous pouvez mettre en évidence le contenu qui s’affiche dans une zone mise en surbrillance. Vous pouvez choisir d’identifier le contenu de cette zone avec un préfixe commun :

- `spotlight_headline`
- `spotlight_body`

Chaque section ne peut avoir qu’un seul type de champ. Par exemple, l’exemple de groupe ci-dessus avec le préfixe `spotlight` ne peut avoir qu’un seul champ `spotlight_headline`.

Lorsque vous avez plusieurs sections (trois max.) :

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

GenStudio comprend que `spotlight_headline` est plus étroitement lié à `spotlight_body` qu’à `news_body`.

+++Exemple : modèle avec plusieurs sections

L’exemple ci-dessous présente le même modèle d’HTML que celui illustré ci-dessus, mais avec deux sections supplémentaires. L’en-tête contient une page CSS intégrée pour le style d’une capsule. Le corps utilise deux capsules avec des espaces réservés de contenu à l’aide d’un préfixe.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
        <div class="pod">
            <h2>{{ pod1_headline }}</h2>
            <p>This is Pod 1 content.</p>
        </div>
        <div class="pod">
            <h2>{{ pod2_headline }}</h2>
            <p>This is Pod 2 content.</p>
        </div>
    </div>
</body>
</html>
```

+++

## Aperçu du modèle

Les modèles de courrier électronique contiennent parfois du contenu spécial qu’il n’est pas nécessaire de prévisualiser dans GenStudio. Vous pouvez contrôler la visibilité de ce contenu à l’aide des assistants intégrés, qui sont des expressions spéciales dans le langage de modèle Handlebars qui permettent d’effectuer certaines actions.

La valeur `_genStudio.browser` est définie lors du rendu d’un modèle et la valeur `genStudio.export` est définie lors de l’exportation d’un modèle. Vous pouvez décider d’inclure certains contenus dans la partie supérieure des emails à l’aide d’un wrapper conditionnel, par exemple, lorsque le modèle est utilisé pour l’exportation :

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un autre exemple peut être d’empêcher l’utilisation des codes de suivi lors de la prévisualisation d’un modèle d’email dans GenStudio. Cet exemple montre comment ajouter des paramètres de suivi aux liens dans le modèle exporté, tout en conservant les liens d’aperçu propres :

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Contenu statique

Les modèles de courrier électronique et de métadonnées sont souvent liés à des images et à des fichiers CSS hébergés en dehors de GenStudio. Lorsque GenStudio génère des miniatures pour ces modèles ou les expériences qui en découlent, il se peut qu’il ignore ces ressources externes si elles ne comportent pas les en-têtes CORS (Cross-Origin Resource Sharing) corrects.

Pour vous assurer que ces ressources sont disponibles pendant le processus de génération de miniatures, envisagez deux options :

1. **Utiliser les en-têtes CORS** : le serveur hôte doit envoyer des réponses avec un en-tête `Access-Control-Allow-Origin` défini sur la valeur `https://experience.adobe.com` pour les environnements de production. Cette méthode permet à GenStudio d’accéder aux ressources et de les inclure.
1. **Utiliser des URL de données** : incorporez les ressources externes directement dans le modèle à l’aide des URL de données. Cette méthode contourne les restrictions CORS et garantit que les ressources sont disponibles pendant la génération des miniatures.
