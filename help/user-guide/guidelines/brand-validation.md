---
title: Validation de marque dans GenStudio
description: Découvrez le fonctionnement du système intégré de validation de marque dans GenStudio.
feature: Brands Service, Guidelines
source-git-commit: c8fa0cf1633a5ca0ab94d9a0f33d9b7e7d6d61ed
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---


# Validation de marque

Dans GenStudio, la validation de la marque est un composant essentiel qui fonctionne en collaboration avec la fonctionnalité et les directives d’IA générative : [[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) et [[!DNL Personas]](/help/user-guide/guidelines/personas.md). Cela garantit que tout votre contenu s’aligne sur votre identité de marque.

GenStudio effectue la validation de la marque sur divers aspects, notamment :

* Indications de marque spécifiques à chaque client
* Copie des directives pour différentes plateformes de canal
* Considérations éthiques liées au genre, à l’ethnie, à la race, au statut d’invalidité et à l’âge dans les contenus générés par l’IA

## Vérification des directives sur les marques

Un résumé des informations de validation de marque pour chaque variante de contenu généré est accessible via l’icône _Vérification des directives de marque_ en regard de chaque variante dans la zone de travail.

La _vérification des directives de marque_ affiche le pourcentage de conformité à votre [marque](brands.md). Le pourcentage est calculé sous la forme du nombre de [consignes](overview.md) ayant réussi la validation par rapport au nombre de consignes testées.

Cliquez sur l’icône pour voir quelles directives sont conformes à votre marque et lesquelles doivent être examinées.

Voir [Améliorer l&#39;alignement de la marque](#improve-brand-alignment).

## Panneau de validation des marques

Le _panneau de validation de marque_ fournit des informations détaillées sur la validation de marque et éclaire les opportunités d’amélioration pour chaque fragment de variante.

Le _panneau de validation de marque_ affiche des informations sur :

* **Email** :
   * Fragment de ligne d’objet
   * Fragment de prétitre
   * Fragment d’en-tête
   * Fragment de contenu
   * Fragment CTA (appel à l’action)
   * Indications pour la marque et la voix
* **Méta-publicité** :
   * Fragment de titre
   * Fragment de copie de contenu
   * Fragment CTA (appel à l’action)
   * Fragment de texte sur image

Voir [Améliorer l&#39;alignement de la marque](#improve-brand-alignment).

### Filtre

Dans le _panneau de validation de marque_, vous pouvez filtrer les directives affichées. Cliquez sur l’icône de filtre en haut du panneau pour afficher :

* **Failed guidelines**—_Show failed guidelines_ affiche uniquement les consignes qui n’ont pas réussi la validation de marque.
* **Toutes les instructions**—_Afficher les instructions transmises et ayant échoué_ affiche toutes les instructions pour lesquelles les variantes sont mesurées.
* **Directives transmises**—_Afficher les consignes transmises_ affiche uniquement les consignes ayant réussi la validation de la marque.

<!-- The _Brand validation panel_ has different areas of focus for each content channel:

* Email - brand voice and channel compliance
* Images - application photography restrictions and other considerations -->

## Améliorer l&#39;alignement des marques

Pour optimiser l’efficacité du contenu généré et maintenir une identité de marque cohérente, utilisez la _vérification des directives de marque_ et le _panneau Validation de marque_. Vous pouvez modifier manuellement des fragments spécifiques pour vous aligner sur les [directives de marque](brands.md).

**Pour améliorer l’alignement de la marque pour les variantes de contenu générées** :

1. Cliquez sur l’icône **[!UICONTROL [!DNL Brand]de vérification de directives]** pour une variante individuelle.

   Affichez un résumé des performances de cette variante spécifique (des instructions qui transmettent la validation de la marque et celles qui doivent être examinées) lorsqu’elle est comparée à votre marque.

1. Pour obtenir les détails des fragments et des directives qui doivent être améliorés, cliquez sur **[!UICONTROL Réviser]** _ou_ cliquez sur l’icône Validation de marque dans la barre de menu supérieure pour ouvrir le _panneau de validation de marque_.

   Consultez tous les fragments et les directives sur la marque qui nécessitent votre attention. Le fragment surligné dans le panneau correspond au fragment surligné dans la variante générée dans la zone de travail.

   >[!NOTE]
   >
   > La directive _Brand voice_ notée dans le _panneau de validation de marque_ s’applique à la variante entière, et non à un fragment individuel. Toute la variante de contenu est mise en surbrillance pour l’amélioration suggérée.

1. Révisez manuellement les fragments de variante pour obtenir l’alignement le plus fort possible sur votre marque.

1. Après avoir effectué les modifications nécessaires, cliquez sur **[!UICONTROL Révérifier]** pour valider vos modifications et vous assurer qu’elles sont plus étroitement alignées sur l’identité de votre marque.

   Le processus de validation de marque s’exécute à nouveau. Si le fragment/la consigne est validé, une coche verte s’affiche pour ce fragment dans le _panneau de validation de marque_. Le pourcentage de l&#39;icône _Vérification de la marque_ pour la variante révisée indique également votre progression.

1. Poursuivez la révision des fragments pour vous assurer que l’ensemble de la variante passe la validation de la marque.

   Naviguez entre les instructions du _panneau de validation de marque_ à l’aide des boutons **[!UICONTROL Suivant]** et **[!UICONTROL Précédent]** .

1. Dans la partie supérieure du _panneau de validation de marque_, naviguez dans chaque variante à l’aide des flèches (par exemple, utilisez la flèche pour passer de `Email 1` à `Email 2`) et continuez à réviser les fragments afin de mieux se conformer à votre marque.

   Pour plus d’informations sur les consignes prises en compte, voir [Brand voice Guidelines](/help/user-guide/guidelines/brands.md#brand-voice-guidelines) .
