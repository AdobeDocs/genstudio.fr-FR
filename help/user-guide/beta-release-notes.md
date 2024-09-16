---
title: Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio pour les marketeurs de performance.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: d1904bfe6e5775f71290c2fc7aa185ac2a4a4668
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta

Ces notes mettent en évidence un Adobe GenStudio important pour les correctifs et améliorations des marketeurs de performance pour la semaine se terminant le 13 septembre.

## Améliorations

* Le sélecteur de contenu [!DNL Create] a été restructuré afin d’améliorer le chargement des ressources. <!-- GS-2586 -->

## Problèmes connus

Les problèmes connus suivants sont programmés pour la résolution dans la version GA de GenStudio pour les marketeurs de performance.

* Les problèmes de latence intermittente affectent certaines opérations [!DNL Create] Canvas. <!-- GS-5203 -->

* La génération de courriers électroniques génère un courrier électronique incomplet. **Solution de contournement** : actualisez la page et régénérez-la. <!-- GS-5209 -->

* Les modèles peuvent être chargés, mais ils ne sont pas visibles. **Solution de contournement** : créez ou téléchargez une ressource et saisissez un nom de groupe de ressources dans le champ **[!UICONTROL Campagnes]**. L’affectation de la ressource à un [!DNL Campaign] ajoute la valeur de métadonnées du nom de groupe. Ensuite, chargez à nouveau le modèle. <!-- GS-4815 -->

* Les miniatures de campagne sont absentes de [!DNL Insights]. <!-- GS-4648 -->

* Les utilisateurs doivent se connecter deux fois à un compte Meta Ads de canal lorsqu’ils sont également connectés à Facebook. **Solution** : déconnectez-vous de Facebook avant de vous connecter à un compte de métadonnées de canal. <!-- GS-4806 -->

### Améliorations supplémentaires et problèmes résolus

* Le canevas [!DNL Create] effectue désormais correctement le rendu des images dans les métadonnées publicitaires. <!-- GS-4864 -->

* Bien que des incohérences puissent exister entre les aperçus du canevas de métadonnées et les vues exportées, les expériences exportées fonctionnent comme prévu. <!-- GS-4492 4401 -->

* Les images téléchargées incluent désormais les balises intelligentes attendues. <!-- GS-4856 -->

* Le fichier CSV d’exportation de métadonnées contient désormais des images comme prévu. Auparavant, le fichier ZIP contenait le fichier d’exportation CSV et les fichiers NULL au lieu des images.  <!-- GS-5107 -->

* Les utilisateurs peuvent désormais saisir du texte dans le champ **[!UICONTROL Téléchargé par]** de la vue Détails du modèle, comme prévu. L’icône de chargement empêchait auparavant les utilisateurs de saisir du texte. <!-- GS-4887 -->

* Une fois la marque supprimée, les utilisateurs ne sont plus redirigés vers la vue Détails. <!-- GS-2663 -->

* Les éditeurs ne reçoivent plus l’erreur suivante lors de l’envoi de variantes pour révision et approbation : `You have no access to view comments on this Object`. <!-- GS-5140 -->

* Mise à jour du modèle d&#39;email utilisé par le workflow de vérification et de validation. <!-- GS-5239 -->

* GenStudio affiche désormais un message d’erreur lorsqu’une erreur réseau se produit lors du chargement du sélecteur de modèles. <!-- GS-4682 -->

* Résolution de problèmes liés à la navigation d’une ressource, d’une expérience ou d’une carte de modèle vers l’objet sélectionné. <!-- GS-4390 -->

* La fenêtre contextuelle _Ajouter Assets_ est désormais localisée lorsqu’elle est ouverte à partir de la zone de travail Créer un canevas.  <!-- GS-4867 -->

* La validation de la marque est désormais déclenchée pour les variantes régénérées. Auparavant, si un éditeur régénérait les variantes d’un brouillon existant, la validation n’était pas déclenchée. <!-- GS-3971 -->

## Versions Beta précédentes

Les versions précédentes de Beta incluaient les mises en évidence et correctifs suivants.

### Tons clairs

* GenStudio prend désormais en charge l’option de prévisualisation des ressources multimédia dans les vues de table et de galerie [!DNL Insights]. Les miniatures vidéo incluent un bouton **Lire** avec une option silencieuse. <!-- GS-4398 -->

* Les directives relatives aux canaux Instagram et Facebook ont été combinées dans les directives relatives aux métadonnées de marque.

* [!DNL Create] Les éléments de navigation du canevas ont été rationalisés. La page d’entrée [!DNL Create] affiche le panneau de navigation de gauche, mais les utilisateurs utilisent désormais un bouton **[!UICONTROL Précédent]** pour accéder à cet espace à partir d’autres zones de travail [!DNL Create].

* Les éléments de navigation ont été améliorés afin de prendre en charge la cible d’action des utilisateurs lors de l’exécution de tâches dans l’ensemble du produit, y compris dans les zones suivantes :

   * Détails des ressources, de l’expérience et des modèles dans [!DNL Content]
   * Expérience, Ressource, Détails des attributs dans [!DNL Insights]
   * Détails de la marque dans [!DNL Brands]
   * Détails du produit et du personnage dans Produits et acteurs impliqués

* Les utilisateurs n’ont plus besoin de cliquer sur le bouton **[!UICONTROL Actualiser]** pour afficher les mises à jour des expériences dans [!DNL Content].

* La page _Détails de l’expérience_ effectue désormais le rendu des miniatures de ressources externes en tant qu’HTML.

* La latence de l’interface utilisateur après l’ajout ou la suppression d’Assets et d’expériences a été améliorée.

* Les aperçus de modèle incluent désormais un texte par défaut plus explicite. Voir [Personnaliser un modèle](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/content/templates/customize-template#template-preview).

* **Score de validation basé sur le pourcentage** : la validation de marque affiche désormais le score de validation de marque sous forme de pourcentage plutôt qu’une valeur de réussite/échec. (fixed 8/16)

* **Interface d’extraction de marque mise à jour** : l’extraction de marque affiche désormais la fin du processus d’extraction sous forme de pourcentage. (fixed 8/16)

* **Chargement incrémentiel de la marque lors de l’extraction** : les directives de marque sont désormais chargées de manière incrémentielle dans l’interface utilisateur. (fixed 8/16)

* **Création d’emails multi-section** : les utilisateurs peuvent désormais créer des emails composés d’éléments distincts pour le titre, l’image, le corps et CTA. (fixed 8/16)

* **MetaAds Resize** : les éditeurs peuvent redimensionner les proportions MetaAd. (fixed 8/16)

* **Comptes de connexion limités [!DNL Insights]** : la connexion [!DNL Insights] ne prend désormais en charge qu’un seul compte par client. (fixed 8/16)

### Améliorations supplémentaires et problèmes résolus

* La fenêtre contextuelle _Ajouter Assets_ est désormais localisée comme prévu. <!-- GS-3834 -->

* Les problèmes de mise à l’échelle du modèle d’expérience Métadonnées ont été résolus. <!-- GS-4174 -->

* Les champs de texte du fichier d’exportation CSV pour les emails en plusieurs parties sont désormais classés comme prévu. <!-- GS-4013 -->

* Le champ de recherche [!DNL Content] ne disparaît plus lorsqu’un utilisateur appuie à plusieurs reprises sur la touche **Retour arrière** pour effacer le texte du champ de recherche.  <!-- GS-4543 -->

* GenStudio pour les spécialistes du marketing des performances charge désormais les utilisateurs comme prévu lorsqu’un collaborateur ajoute une mention `@` à un commentaire. Auparavant, les utilisateurs n’étaient pas chargés et une erreur s’affichait : `Unable to load users. Refresh the page`. <!-- GS-4113 -->

* GenStudio n’affiche plus le message **Une erreur s’est produite** lorsqu’un éditeur clique sur **Sélectionner le contenu** lors de la création de l’email dans la zone d’invite. <!-- GS-4879 -->

* Le nom d’emplacement du flux de page _Détails de l’expérience_ spécifie désormais le flux Facebook ou Instagram. (fixed 8/16)

* Le recadrage d’images et de vidéos plus grandes est désormais cohérent lorsque l’utilisateur navigue de la vue _Présentation de la ressource_ vers la vue _Détails de la ressource_. (fixed 8/16)

* Le nombre de résultats de recherche sur l’écran Attributs n’affiche plus `0 of` avant qu’un utilisateur ne se connecte. (fixe 8/16) <!-- GS-3665 -->

* Cliquer sur le champ de comptage **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** n’efface plus les paramètres de recherche et de filtre. (fixe 8/16) <!-- GS-3476 -->

* GenStudio affiche une erreur lorsqu’un utilisateur tente de saisir des informations d’identification dans la vue [!DNL Insights]. (fixe 8/29) <!-- GS-4689 -->

* Le téléchargement des directives sur la marque échoue en raison de problèmes liés à la plateforme de stockage ACP. (fixe 8/22) <!-- GS-4369 -->

* Le menu déroulant Zone d’invite [!DNL Brands] affiche un compteur à la fin de la liste [!DNL Brands] lors de la création de l’email. (fixe 8/22) <!-- GS-4077 -->
