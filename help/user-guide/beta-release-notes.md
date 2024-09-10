---
title: Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio pour les marketeurs de performance.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 2e40260db0f9972675b103c51f09acbfa83a1cb5
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 0%

---

# Notes de mise à jour d’Adobe GenStudio pour les spécialistes du marketing de performance Beta

Ces notes mettent en évidence un Adobe GenStudio important pour les correctifs et améliorations des marketeurs de performance pour la semaine se terminant le 6 septembre.

## Nouvelles fonctionnalités

* GenStudio prend désormais en charge l’option de prévisualisation des ressources multimédia dans les vues de table et de galerie [!DNL Insights]. Les miniatures vidéo incluent un bouton **Lire** avec une option silencieuse. <!-- GS-4398 -->

## Problèmes connus

Les problèmes connus suivants sont programmés pour la résolution dans la version GA de GenStudio pour les marketeurs de performance.

* Les éditeurs rencontrent parfois un message d’erreur &quot;Une erreur s’est produite&quot; sur le [!DNL Create Canvas] lors de la génération de l’image. **Solution** : si l’erreur se répète, l’utilisateur peut se déconnecter, puis se reconnecter à GenStudio et régénérer l’image.  <!-- GS-4813 -->

* Le [!DNL Create Canvas] effectue un rendu incorrect des images dans les métadonnées publicitaires. <!-- GS-4864 -->

* Assets sans campagnes peut être transféré dans [!DNL Content], mais les utilisateurs peuvent ne pas être visibles. <!-- GS-4815 -->

* Il existe une différence entre les aperçus du canevas de métadonnées et les vues exportées. <!-- GS-4492 4401 -->

* Les miniatures de campagne sont absentes de [!DNL Insights]. <!-- GS-4648 -->

* Les utilisateurs peuvent actuellement sélectionner de petites ressources qui nécessitent un redimensionnement, mais l’agrandissement de ces ressources n’est pas pris en charge. <!-- GS-3131 -->

* Les utilisateurs doivent se connecter deux fois à un compte Meta Ads de canal lorsqu’ils sont également connectés à Facebook. **Solution** : déconnectez-vous de Facebook avant de vous connecter à un compte de métadonnées de canal.

* Les images téléchargées n’incluent pas toujours les balises intelligentes attendues. <!-- GS-4856 -->

### Améliorations supplémentaires et problèmes résolus

* La fenêtre contextuelle _Ajouter Assets_ est désormais localisée comme prévu. <!-- GS-3834 -->

* Les problèmes de mise à l’échelle du modèle d’expérience Métadonnées ont été résolus. <!-- GS-4174 -->

* Les champs de texte du fichier d’exportation CSV pour les emails en plusieurs parties sont désormais classés comme prévu. <!-- GS-4013 -->

* Le champ de recherche [!DNL Content] ne disparaît plus lorsqu’un utilisateur appuie à plusieurs reprises sur la touche **Retour arrière** pour effacer le texte du champ de recherche.  <!-- GS-4543 -->

* GenStudio charge désormais les utilisateurs comme prévu lorsqu’un collaborateur ajoute une mention @ à un commentaire. Auparavant, GenStudio ne chargeait pas les utilisateurs et affichait cette erreur : `Unable to load users. Refresh the page`. <!-- GS-4113 -->

* GenStudio n’affiche plus le message **Une erreur s’est produite** lorsqu’un éditeur clique sur **Sélectionner le contenu** lors de la création de l’email dans la zone d’invite. <!-- GS-4879 -->

## Versions Beta précédentes

Les versions précédentes de Beta incluaient les mises en évidence et correctifs suivants.

### Tons clairs

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

* **Redimensionnement des métadonnées publicitaires** : les éditeurs peuvent redimensionner les proportions des métadonnées publicitaires. (fixed 8/16)

* **Comptes de connexion limités [!DNL Insights]** : la connexion [!DNL Insights] ne prend désormais en charge qu’un seul compte par client. (fixed 8/16)

### Améliorations supplémentaires et problèmes résolus

* Le nom d’emplacement du flux de page _Détails de l’expérience_ spécifie désormais le flux Facebook ou Instagram. (fixed 8/16)

* Le recadrage d’images et de vidéos plus grandes est désormais cohérent lorsque l’utilisateur navigue de la vue _Présentation de la ressource_ vers la vue _Détails de la ressource_. (fixed 8/16)

* Le nombre de résultats de recherche sur l’écran Attributs n’affiche plus `0 of` avant qu’un utilisateur ne se connecte. (fixe 8/16) <!-- GS-3665 -->

* Cliquer sur le champ de comptage **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Asset]** n’efface plus les paramètres de recherche et de filtre. (fixe 8/16) <!-- GS-3476 -->

### Problèmes connus résolus dans les versions précédentes de Beta

* GenStudio affiche une erreur lorsqu’un utilisateur tente de saisir des informations d’identification dans la vue [!DNL Insights]. (fixe 8/29) <!-- GS-4689 -->

* Le téléchargement des directives sur la marque échoue en raison de problèmes liés à la plateforme de stockage ACP. (fixe 8/22) <!-- GS-4369 -->

* Le menu déroulant Zone d’invite [!DNL Brands] affiche un compteur à la fin de la liste [!DNL Brands] lors de la création de l’email. (fixe 8/22) <!-- GS-4077 -->
