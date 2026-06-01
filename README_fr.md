<!--
  CONFIGURATION — remplacez ces deux espaces réservés partout avant la publication :
    {{WEBSITE_URL}}    →  votre site officiel, par ex. https://veo-automation.example.com
    {{EXTENSION_URL}}  →  l'URL de votre fiche sur le Chrome Web Store (sans chaîne de requête)
  Les liens de l'extension ajoutent déjà ?hl={lang} selon le fichier de langue. Effectuez un
  rechercher/remplacer global sur les 7 fichiers README (README.md, README_zh/ko/ja/de/fr/ru.md).
-->

[![Installer depuis le Chrome Web Store](https://img.shields.io/badge/⬇_Installer-Chrome_Web_Store-success?style=for-the-badge&logo=googlechrome&logoColor=white)]({{EXTENSION_URL}}?hl=fr)
[![Site web](https://img.shields.io/badge/🌐_Site_web-Visiter-blue?style=for-the-badge)]({{WEBSITE_URL}})

# 🎬 VEO Automation — Automatisation par lot de Google Flow pour les vidéos VEO 3 et les images Nano Banana

[![English](https://img.shields.io/badge/English-blue)](README.md) [![中文](https://img.shields.io/badge/中文-red)](README_zh.md) [![한국어](https://img.shields.io/badge/한국어-orange)](README_ko.md) [![日本語](https://img.shields.io/badge/日本語-purple)](README_ja.md) [![Deutsch](https://img.shields.io/badge/Deutsch-green)](README_de.md) [![Français](https://img.shields.io/badge/Français-yellow)](README_fr.md) [![Русский](https://img.shields.io/badge/Русский-lightgrey)](README_ru.md)

> **VEO Automation** est l'extension Chrome qui transforme [Google Flow](https://labs.google/fx/tools/flow) en véritable studio de génération par lot. Mettez des centaines de prompts en file d'attente, générez des vidéos **VEO 3** et des images **Nano Banana** en masse, puis téléchargez automatiquement chaque résultat — fini de surveiller un prompt après l'autre.

**Mots-clés couverts par ce guide :** automatisation Google Flow · automatisation VEO · génération par lot VEO 3 · générateur d'images Nano Banana par lot · générateur de vidéos IA en masse · téléchargement automatique des vidéos VEO · extension Chrome Google Flow.

---

## 📑 Table des matières

- [Pourquoi VEO Automation](#-pourquoi-veo-automation)
- [Fonctionnalités clés](#-fonctionnalités-clés)
- [Installation](#-installation)
- [Démarrage rapide](#-démarrage-rapide)
- [Modes de génération](#-modes-de-génération)
- [Référence des paramètres](#-référence-des-paramètres)
- [Astuces et bonnes pratiques](#-astuces-et-bonnes-pratiques)
- [Dépannage](#-dépannage)
- [FAQ](#-faq)
- [Confidentialité et autorisations](#-confidentialité-et-autorisations)
- [Tarifs](#-tarifs)

---

## 🚀 Pourquoi VEO Automation

Google Flow est puissant, mais son interface officielle vous oblige à lancer **un prompt à la fois** et à télécharger **un fichier à la fois**. Si vous produisez du contenu à grande échelle — vidéos courtes, créations marketing, storyboards, visuels produit — cette boucle manuelle devient un véritable goulot d'étranglement.

VEO Automation l'élimine :

- **Collez une liste, puis laissez tourner.** Déposez des dizaines ou des centaines de prompts : l'extension les traite les uns après les autres, avec nouvelle tentative en cas d'échec, pendant que vous faites autre chose.
- **Vidéos VEO 3 *et* images Nano Banana dans un seul outil.** La plupart des automatisations ne touchent qu'à la vidéo. Celle-ci traite par lot à la fois les modèles vidéo de Google Flow et le modèle d'image Nano Banana, depuis un seul panneau latéral.
- **Les fichiers arrivent sur le disque automatiquement.** Chaque vidéo et chaque image terminée est renommée et enregistrée dans un dossier par projet — sans marathon de clic-droit-enregistrer.

Si vous cherchiez un *outil de génération par lot pour Google Flow*, un *générateur en masse VEO 3*, ou un moyen de *télécharger automatiquement vos images Nano Banana*, c'est exactement pour cela que cet outil a été conçu.

---

## ✨ Fonctionnalités clés

| Fonctionnalité | Ce qu'elle fait |
| --- | --- |
| 🚀 **File d'attente par lot** | Ajoutez un nombre illimité de prompts à la liste d'attente ; les tâches s'exécutent les unes après les autres, automatiquement. |
| 📝 **Texte vers vidéo (VEO 3)** | Collez vos prompts ou importez un fichier `.txt` de centaines de lignes pour produire des vidéos en masse. |
| 🖼️ **Image vers vidéo (VEO 3)** | Animez des images fixes grâce au contrôle image de départ / image de fin. |
| 🎨 **Texte vers image (Nano Banana)** | Générez des images à partir de descriptions textuelles, en masse. |
| 🔄 **Image vers image (Nano Banana)** | Transformez ou retouchez des images de référence à grande échelle. |
| 💾 **Téléchargement automatique** | Enregistre instantanément les vidéos et images terminées sur votre machine, organisées par dossier de projet. |
| 🔁 **Nouvelle tentative automatique** | Un souci réseau ou une « échec de création » du côté de Google ? L'outil patiente et réessaie automatiquement. |
| 🔗 **Enchaînement de clips (concat)** | Assemblez des segments de 8 secondes en vidéos continues plus longues. |
| ⚙️ **Personnalisation poussée** | Choisissez le modèle, le format d'image (16:9 / 9:16 / 1:1), le nombre de sorties par prompt (1 à 4), l'exécution simultanée et le délai entre prompts. |
| 🌍 **7 langues** | English, 中文, 한국어, 日本語, Deutsch, Français, Русский. |

---

## 📥 Installation

### Chrome Web Store (recommandé)

1. Ouvrez la [**fiche VEO Automation**]({{EXTENSION_URL}}?hl=fr) sur le Chrome Web Store.
2. Cliquez sur **Ajouter à Chrome** → **Ajouter l'extension**.
3. Épinglez l'extension : cliquez sur l'icône en forme de pièce de puzzle dans la barre d'outils de Chrome, puis sur l'épingle à côté de **VEO Automation**, pour l'avoir à portée d'un clic la prochaine fois.

> **Compatibilité :** Chrome 137+ (et les navigateurs basés sur Chromium comme Edge et Brave). L'extension s'ouvre sous forme de **panneau latéral** à côté de Google Flow.

---

## ⚡ Démarrage rapide

1. **Ouvrez Google Flow.** Rendez-vous sur [labs.google/fx/tools/flow](https://labs.google/fx/tools/flow) et ouvrez (ou créez) un projet. L'extension ne s'active que sur les pages de projet Flow.
2. **Ouvrez le panneau latéral.** Cliquez sur l'icône VEO Automation. Connectez-vous pour débloquer votre quota quotidien.
3. **Choisissez un mode.** Sélectionnez l'un des cinq modes de génération (ci-dessous).
4. **Ajoutez vos prompts.** Saisissez-les, ou importez un fichier `.txt`.
5. **Cliquez sur Lancer.** Regardez la file d'attente traiter chaque tâche, réessayer en cas d'erreur et télécharger automatiquement les résultats.

> ℹ️ **À propos de la bannière de « débogage ».** Pendant que l'extension fonctionne, Chrome affiche en haut une barre indiquant *« … est en cours de débogage »*. C'est indispensable : Google Flow n'accepte que des entrées utilisateur authentiques et de confiance, l'extension pilote donc la page via l'interface de débogage officielle de Chrome. Ce n'est pas un logiciel malveillant — c'est le prix d'une automatisation fiable. Ne fermez pas cette bannière pendant qu'un lot est en cours.

---

## 🎛️ Modes de génération

### 1. Texte vers vidéo — VEO 3

Produisez des vidéos en masse directement à partir de texte.

1. Sélectionnez **Texte vers vidéo**.
2. Saisissez vos prompts dans le champ (séparez chaque prompt par une **ligne vide**) **ou** cliquez sur **Importer .txt** pour charger une liste de prompts.
3. Définissez la durée (clip unique de 8 s, ou **Concat** pour des vidéos enchaînées plus longues).
4. Cliquez sur **Lancer**.

**Exemple de liste de prompts :**

```
Un phare solitaire sur une falaise à l'heure dorée, des vagues se brisant en contrebas, lent travelling avant cinématographique.

Une ruelle de Tokyo aux néons sous la pluie, reflets sur l'asphalte mouillé, vapeur qui s'élève, caméra à l'épaule.

Vue aérienne glissant au-dessus d'une forêt d'automne, brume matinale basse entre les arbres, lumière chaude.
```

### 2. Image vers vidéo — VEO 3

Donnez vie à vos images fixes.

1. Sélectionnez **Image vers vidéo**.
2. Cliquez sur **Sélectionner des images** (sélection multiple prise en charge) et faites glisser pour réordonner par nom, date ou ordre personnalisé.
3. Écrivez un prompt par image (séparés par une ligne vide).
4. Choisissez la durée, puis **Lancer**.

> **Astuce :** Utilisez une image de départ + une image de fin pour contrôler le début et la fin du mouvement. Configurez 1 à 2 images par prompt dans les Paramètres.

### 3. Texte vers image — Nano Banana

Générez des images à partir de descriptions, en masse.

1. Sélectionnez **Texte vers image**.
2. Saisissez des prompts d'image détaillés (séparés par une ligne vide).
3. Définissez le format d'image et la qualité d'image dans les Paramètres.
4. **Lancez** — chaque image se télécharge automatiquement à la résolution choisie (1K / 2K / 4K).

### 4. Image vers image — Nano Banana

Retouchez ou restylisez des images de référence à grande échelle.

1. Sélectionnez **Image vers image**.
2. Importez vos images sources.
3. Écrivez des prompts de transformation (par ex. *« même personnage, tenue cyberpunk, sur un toit la nuit »*).
4. **Lancez** pour générer des variantes basées sur vos références.

> **Association automatique des personnages par nom de fichier (facultatif) :** nommez vos références `chien.png`, `chat.png`, `canard.png`. Un prompt qui mentionne *« un chien qui joue avec un chat »* importe automatiquement `chien.png` et `chat.png`. Idéal pour garder vos personnages cohérents tout au long d'une série.

### 5. Gestion de la file d'attente

- Visualisez chaque tâche en attente dans la **File d'attente des prompts**.
- **Supprimez** les tâches dont vous n'avez plus besoin, ou **Arrêtez** un lot en cours d'exécution.
- Suivez la progression en temps réel pour chaque prompt.

---

## ⚙️ Référence des paramètres

Ouvrez l'onglet **Paramètres** pour ajuster le comportement.

**Général**
- **Mode par défaut** — sélectionné automatiquement à chaque ouverture du panneau.
- **Format d'image par défaut** — 16:9, 9:16 ou 1:1.
- **Sorties par prompt** — 1 à 4 vidéos/images par prompt.
- **Prompts simultanés** — exécutez 1 à 6 prompts en même temps.
- **Délai entre prompts** — patientez de 0 à 300 s entre les prompts pour ménager la charge du serveur.

**Modèles**
- **Modèle vidéo** — choisissez votre modèle VEO (par ex. VEO 3 / VEO 3 Fast).
- **Modèle d'image** — Nano Banana pour le texte vers image et l'image vers image.

**Téléchargement**
- **Qualité vidéo** — 720p, 1080p, ou désactivé.
- **Qualité d'image** — 1K, 2K, 4K, ou désactivé.
- Les fichiers sont enregistrés dans le dossier Téléchargements de Chrome, un sous-dossier par projet.

**Avancé**
- **Nombre maximal de tentatives** — 1 à 20 essais en cas d'échec.
- **Cadrage vidéo par défaut** — 8 s ou Concat.
- **Nombre maximal d'images par prompt** — à définir par mode.
- **Langue** — basculez l'interface entre 7 langues.

---

## 💡 Astuces et bonnes pratiques

**Rédiger des prompts**
- Soyez précis sur le sujet, le style, les mouvements de caméra et l'éclairage.
- Les prompts en anglais sont généralement les plus fiables sur Google Flow.
- Séparez les prompts par une seule ligne vide.

**Débit vs stabilité**
- Heures creuses : environ 3 prompts simultanés fonctionnent bien.
- Heures de pointe : descendez à 2 et augmentez le délai à environ 30 s — moins d'erreurs « échec de création ».
- Plus d'exécution simultanée = plus rapide mais moins stable ; ajustez selon vos besoins.

**Gérer les ressources**
- Nommez clairement vos images de référence pour que l'association automatique fonctionne.
- Privilégiez les formats PNG / JPG / GIF, idéalement sous 10 Mo chacun.

**Fiabilité**
- Laissez la **Nouvelle tentative automatique** activée pour les lots de nuit sans surveillance.
- Un délai plus élevé = charge serveur allégée = moins d'échecs.

---

## 🔧 Dépannage

| Symptôme | Cause et solution |
| --- | --- |
| **L'extension ne fait rien** | Vous devez être sur une page de **projet** Google Flow. Vérifiez que l'extension est activée, actualisez la page et rouvrez le panneau. |
| **« Impossible de créer la vidéo »** | Google Flow est temporairement surchargé. Pas d'inquiétude — l'extension patiente et réessaie toutes les ~30 s jusqu'à ce qu'un créneau se libère. |
| **Les vidéos/images ne se téléchargent pas** | Dans Chrome : **Paramètres → Téléchargements → désactivez** *« Toujours demander où enregistrer les fichiers avant de les télécharger. »* Puis revérifiez la qualité de téléchargement dans les Paramètres. |
| **« Erreur de politique »** | Votre prompt ou votre image a déclenché la politique de contenu de Google. L'outil ignore cette tâche et passe automatiquement à la suivante. |
| **La génération échoue en continu** | Vérifiez votre connexion, assurez-vous que les prompts sont valides, augmentez le nombre maximal de tentatives et consultez la console du navigateur pour plus d'indices. |
| **La page a dézoomé toute seule** | C'est intentionnel — l'outil ajuste le zoom afin de localiser les boutons avec précision. Ne modifiez pas le zoom manuellement pendant qu'un lot s'exécute. |
| **La bannière « en cours de débogage » ne disparaît pas** | Normal pendant l'exécution (voir Démarrage rapide). Elle disparaît à la fin du lot ou lorsque vous l'arrêtez. |

---

## ❓ FAQ

**VEO Automation est-il affilié à Google ?**
Non. C'est un outil tiers indépendant qui automatise l'application web publique Google Flow. Il n'est ni affilié, ni approuvé, ni lié à Google.

**Qu'est-ce que Nano Banana ?**
Nano Banana est le modèle d'image accessible via Google Flow. VEO Automation vous permet de générer par lot et de télécharger automatiquement les images Nano Banana en même temps que vos vidéos VEO 3 — depuis la même file d'attente.

**Puis-je vraiment générer des centaines de vidéos d'un coup ?**
Oui. Importez un fichier `.txt` de prompts (ou collez une longue liste) et la file d'attente les traite un par un, avec nouvelle tentative automatique. Le débit réel dépend de la charge de Google Flow ainsi que de vos réglages d'exécution simultanée et de délai.

**Cela fonctionne-t-il pour la vidéo verticale au format court ?**
Oui — réglez le format d'image sur **9:16** pour TikTok / Reels / Shorts, **16:9** pour YouTube, ou **1:1** pour le carré.

**Où vont mes fichiers ?**
Dans votre dossier Téléchargements de Chrome, organisés en un sous-dossier par projet et renommés automatiquement pour être faciles à trier.

**Ai-je besoin d'une clé API ?**
Non. L'outil pilote votre propre session Google Flow connectée dans le navigateur — aucune clé API ni compte développeur distinct n'est requis.

**Mes données sont-elles envoyées quelque part ?**
Vos prompts, images et vidéos sont traités dans votre navigateur sur Google Flow. L'extension stocke les paramètres localement. Voir [Confidentialité et autorisations](#-confidentialité-et-autorisations).

**Quels navigateurs sont pris en charge ?**
Chrome 137+ et les navigateurs basés sur Chromium (Edge, Brave). Un panneau latéral est requis.

---

## 🔒 Confidentialité et autorisations

- **Tout s'exécute dans votre navigateur.** L'automatisation se déroule sur votre propre session Google Flow.
- **Données minimales.** Les paramètres sont stockés dans le stockage local de Chrome. L'extension ne vend ni ne collecte vos contenus créatifs.
- **Autorisations limitées.** L'accès aux hôtes se restreint à `labs.google/*` (pour automatiser Flow) et au backend propre à l'extension (pour la connexion et le quota).
- **L'autorisation de débogage** sert uniquement à envoyer des événements d'entrée de confiance à Google Flow, ce que la page exige — voir [Démarrage rapide](#-démarrage-rapide).

Tous les détails : [{{WEBSITE_URL}}]({{WEBSITE_URL}})

---

## 💳 Tarifs

VEO Automation est **freemium** :

- **Gratuit** — un quota de génération quotidien qui se réinitialise chaque jour. Parfait pour tester l'outil et pour un usage léger.
- **Pro** — un quota plus élevé ou illimité pour les utilisateurs intensifs lançant de gros lots.

Connectez-vous dans le panneau latéral pour voir votre quota actuel. Gérez votre abonnement sur [{{WEBSITE_URL}}]({{WEBSITE_URL}}).

---

## 🌐 Liens

- **Installer :** [Chrome Web Store]({{EXTENSION_URL}}?hl=fr)
- **Site web :** [{{WEBSITE_URL}}]({{WEBSITE_URL}})
- **Google Flow :** [labs.google/fx/tools/flow](https://labs.google/fx/tools/flow)

---

_Avertissement : VEO Automation est un projet indépendant et n'est **pas** affilié, approuvé ni lié à Google ou à l'équipe Google Flow. « VEO », « Nano Banana », « Google Flow » et « Google » sont des marques de Google LLC. L'utilisation de cet outil est soumise aux conditions d'utilisation de Google._
