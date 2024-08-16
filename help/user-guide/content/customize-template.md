---
title: Personnalisation des modèles
description: Découvrez comment créer un modèle personnalisé pour Adobe GenStudio pour les spécialistes du marketing des performances.
level: Intermediate
feature: Templates, Content
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---


# Personnalisation des modèles

Adaptez vos modèles d’HTML pour Adobe GenStudio pour les spécialistes du marketing des performances à l’aide du langage de modèle _Handlebars_. La syntaxe Handlebars utilise du texte normal avec des accolades doubles comme espaces réservés au contenu. Voir [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) dans le _guide de langue Handlebars_ pour apprendre à préparer votre modèle.

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->If you do not have an HTML template ready to use in GenStudio for Performance Marketers, you can start by defining the structure of your email using HTML tags: `DOCTYPE`, `html`, `head`, and `body`. You can include CSS styles to customize the appearance of your email.

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

Voir [Exemples de modèles](#template-examples).

>[!TIP]
>
>Dans les sections suivantes, ajoutez des espaces réservés de contenu pour les champs d’email, reportez-vous aux exemples de modèles, masquez les éléments superflus de l’aperçu et gérez les liens vers du contenu statique. Une fois votre modèle prêt, vous pouvez [le charger vers GenStudio pour les marketeurs de performances](use-templates.md#upload-a-template) et commencer à générer des emails personnalisés basés sur votre modèle personnalisé.

## Espaces réservés de contenu

Dans l’en-tête ou dans le corps d’un modèle, vous pouvez utiliser la syntaxe des Guidons pour insérer des espaces réservés de contenu dans lesquels vous avez besoin de GenStudio pour que les marketeurs de performance renseignent le modèle avec du contenu réel. GenStudio pour les spécialistes du marketing des performances reconnaît et interprète automatiquement les espaces réservés de contenu en fonction du nom du champ.

Par exemple, vous pouvez utiliser `{{ headline }}` pour indiquer où le titre de l&#39;email doit être placé :

```handlebars
<div>{{ headline }}</div>
```

### Noms de champ

Le nombre maximal de champs autorisés dans un modèle personnalisé est de vingt.

#### Noms de champ reconnus

Le tableau suivant répertorie les noms de champ reconnus par GenStudio pour les spécialistes du marketing des performances pour la population dans les modèles.

| Champ | Rôle | Modèle de canal |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | En-tête pre | email (recommandé) |
| `headline` | Titre | email (recommandé)<br>Métadonnées |
| `body` | Copie de contenu | email (recommandé)<br>Métadonnées |
| `cta` | Appel à l’action | email (recommandé)<br>Métadonnées |
| `on_image_text` | Sur le texte de l’image | Métadonnées publicitaires (recommandé) |
| `image` | Image | email (recommandé)<br>Métadonnées (recommandé) |
| `brand_logo` | Logo de la marque sélectionnée | email<br>Métadonnées |

GenStudio pour les spécialistes du marketing des performances renseigne automatiquement certains champs dans les modèles. Il n’est donc pas nécessaire de les inclure dans vos conceptions de modèle :

* Champ `subject` (modèle d&#39;email)
* Champs `headline`, `body` et `CTA` (modèle de métadonnées publicitaires)

>[!WARNING]
>
>Pour les annonces Instagram, le titre généré n’apparaît pas dans l’expérience finale.

#### Nom du champ du logo de la marque

Pour ajouter un logo de marque dans votre modèle, utilisez l’une des méthodes suivantes pour effectuer le rendu du logo par défaut.

_Exemple_ :

```bash
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default image>{{/if}}" alt="WKND" style="max-width: 88px; margin: 10px auto; display: block;"> 
```

_Exemple_ :

```bash
{{#if brand_logo}}

                    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">

                {{else}}

                    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">

                {{/if}}
```

#### Noms de champ manuels

Tous les autres noms de champ sont traités comme des champs renseignés manuellement. Si vous souhaitez qu’une section soit modifiable, ajoutez des crochets doubles autour de la section à modifier.

_Exemple_ : ``{{customVariable}}`` (`customVariable` est la section modifiable manuellement)

## Sections ou groupes

Les _sections_ informent GenStudio for Performance Marketing que les champs de cette section nécessitent un haut degré de cohérence. L’établissement de cette relation permet à l’IA de générer du contenu qui correspond aux éléments créatifs de la section .

Utilisez un préfixe de votre choix dans le nom du champ pour indiquer qu’un champ fait partie d’une section ou d’un groupe.

Par exemple, vous pouvez mettre en évidence le contenu qui s’affiche dans une zone mise en surbrillance :

* `spotlight_headline`
* `spotlight_body`

Chaque section ne peut comporter qu’un seul type de champ. Dans l’exemple ci-dessus, le préfixe `spotlight` ne peut comporter qu’un seul champ `spotlight_headline`.

Un modèle peut comporter trois sections au maximum :

* `headline`
* `body`
* `spotlight_headline`
* `spotlight_body`
* `news_headline`
* `news_body`

GenStudio pour les spécialistes du marketing des performances comprend que `spotlight_headline` est plus étroitement lié à `spotlight_body` qu’à `news_body`.

## Exemples de modèles

+++Exemple : modèle d&#39;email avec une section

Voici un exemple de base d&#39;un modèle d&#39;HTML pour un email contenant une section. L’en-tête contient une feuille CSS simple et intégrée pour la mise en forme. Le corps contient un `pre-header`, un `headline` et un `image` [espace réservé](#content-placeholders) à utiliser par GenStudio pour que les marketeurs de performance injectent du contenu pendant le processus de génération de courrier électronique.

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

+++Exemple : modèle d&#39;email avec plusieurs sections

L’exemple ci-dessous présente le même modèle d’HTML que celui illustré ci-dessus, mais avec deux sections supplémentaires. L’en-tête contient des CSS intégrés pour le style d’un groupe. Le corps utilise deux groupes avec des [espaces réservés de contenu](#content-placeholders) à l’aide d’un préfixe.

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

+++Exemple : modèle de métadonnées publicitaires

Voici un exemple de base d’un modèle de métadonnées publicitaires. L’en-tête contient des CSS intégrés pour la mise en forme. Le corps utilise des [espaces réservés de contenu](#content-placeholders) à l’aide d’un préfixe.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>

</body>
</html>
```

+++

## Aperçu du modèle

Contrôlez la visibilité du contenu spécial à l’aide des assistants intégrés (expressions spéciales dans le langage de modèle Handlebars qui effectuent certaines actions). Par exemple, vous pouvez ajouter des paramètres de suivi aux liens dans le modèle exporté tout en conservant les liens d’aperçu propres.

La valeur `_genStudio.browser` est définie lors du rendu d’un modèle et la valeur `genStudio.export` est définie lors de l’exportation d’un modèle. Vous pouvez décider d’inclure certains contenus en haut d’un email à l’aide d’un wrapper conditionnel, par exemple, lorsque le modèle est utilisé pour l’exportation :

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un autre exemple peut être d’empêcher l’utilisation des codes de suivi lors de la prévisualisation d’un modèle dans GenStudio. Cet exemple montre comment ajouter des paramètres de suivi aux liens dans le modèle exporté, tout en conservant les liens d’aperçu propres :

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Contenu statique

Les modèles de courrier électronique et de métadonnées sont souvent liés à des images et à des fichiers CSS hébergés en dehors de GenStudio pour les marketeurs de performances. Lorsque GenStudio pour les spécialistes du marketing des performances génère des miniatures pour ces modèles ou les expériences qui en découlent, il se peut que ces ressources externes soient ignorées si elles ne comportent pas les en-têtes CORS (Cross-Origin Resource Sharing) corrects.

Pour vous assurer que ces ressources sont disponibles pendant le processus de génération de miniatures, envisagez deux options :

1. **Utiliser les en-têtes CORS** : le serveur hôte doit envoyer des réponses avec un en-tête `Access-Control-Allow-Origin` défini sur la valeur `https://experience.adobe.com` pour les environnements de production. Cette méthode permet à GenStudio pour les marketeurs de performances d’accéder aux ressources et de les inclure.
1. **Utiliser des URL de données** : incorporez les ressources externes directement dans le modèle à l’aide des URL de données. Cette méthode contourne les restrictions CORS et garantit que les ressources sont disponibles pendant la génération des miniatures.
