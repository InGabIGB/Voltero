<div align="center">

# ⚡ VOLTERO — Projet Voltaire AIO

**Suite complète d'automatisation et d'assistance IA pour Projet Voltaire (PC & Tablette)**

[![Installer sur Greasy Fork](https://img.shields.io/badge/Greasy%20Fork-Install%201--Clic%20(v18.0)-brightgreen?style=for-the-badge&logo=tampermonkey)](https://greasyfork.org/fr/scripts/607368-voltero-projet-voltaire-aio)
[![GitHub Releases](https://img.shields.io/badge/GitHub-Releases%20(.user.js)-181717?style=for-the-badge&logo=github)](../../releases/latest)
[![IA Support](https://img.shields.io/badge/IA-Groq%20%26%20Gemini-blueviolet?style=for-the-badge)](https://console.groq.com/keys)
[![Plateformes](https://img.shields.io/badge/Support-PC%20%7C%20Tablette%20%7C%20Mobile-blue?style=for-the-badge)](#-installation)

[**🌐 Option 1 : Installer depuis Greasy Fork**](https://greasyfork.org/fr/scripts/607368-voltero-projet-voltaire-aio) • [**📦 Option 2 : Télécharger via les Releases**](../../releases/latest)

</div>

---

## 🎯 Présentation

**VOLTERO** est un userscript tout-en-un conçu pour **Projet Voltaire** (`apprentissage.appli1.projet-voltaire.fr`). Doté d'une interface flottante **UI Aurora**, il combine un moteur de résolution par intelligence artificielle (**Groq** et **Google Gemini**), une mémoire locale auto-apprenante à latence nulle (`0 ms`) et des outils anti-détection avancés.

> ⚠️ **Sécurité & Clés API :** Aucune clé API n'est intégrée dans le code source. Tu dois renseigner ta propre clé gratuite **Groq** (`gsk_...`) ou **Google Gemini** (`AIza...`) directement dans les paramètres de l'interface.

---

## ✨ Fonctionnalités principales

### 🎭 4 Modes d'assistance au choix
* **Auto :** Résout l'exercice et clique automatiquement sur la bonne réponse.
* **Vert :** Surligne discrètement la bonne réponse en vert sans cliquer à ta place.
* **1..6 :** Affiche uniquement un petit numéro discret en bas à gauche de l'écran (Vocabulaire & Expression).
* **Boîte :** Affiche la solution uniquement à l'intérieur du HUD de la fenêtre VOLTERO.

### 🧠 Support complet & Moteur DOM optimisé
* **Orthographe :** Détection instantanée des fautes dans les phrases et QCM.
* **Vocabulaire & Expression :** Analyse des synonymes, définitions et nuances de sens.
* **Tableaux *Cliquer / Déposer* :** Classement automatique dans les bonnes colonnes avec **clic `VALIDER` débloqué**.
* **Filtrage des fantômes React Native :** Nettoyage intelligent des nœuds DOM invisibles ou dupliqués pour éviter les faux clics et erreurs de lecture.
* **Mémo grammatical intégré :** Règles complètes des pluriels et exceptions (`-ail`, `-ou`, `-al`, `-eu`) intégrées au moteur d'analyse.

### 🤖 Pool IA Multi-Fournisseurs (Groq & Gemini)
* **Gestionnaire multi-clés :** Ajout illimité de clés `Groq` et `Gemini` avec test de ping et vérification des quotas en direct.
* **Rotation automatique (*Failover*) :** Bascule instantanément sur la clé suivante en cas de limite de débit (`HTTP 429`) ou d'erreur réseau.
* **Auto-Scan (`↻ Sync API`) :** Récupère automatiquement la liste des modèles actifs disponibles sur ton compte.
* **Double vérification IA :** Lance une seconde passe indépendante avant de valider en cas d'ambiguïté.

### ⚡ Mémoire locale auto-apprenante (0 ms)
* Enregistre automatiquement les bonnes réponses **uniquement lorsque Projet Voltaire les valide en vert**.
* Répond instantanément (`0 ms`) sans consommer de tokens API dès qu'une phrase ou un mot déjà vu retombe.
* Onglet dédié permettant de rechercher, filtrer ou supprimer des entrées une par une.

### 🛡️ Timing humain & Anti-détection
* **Taux de réussite réglable (`0 %` à `100 %`) :** Simule des erreurs volontaires pour conserver des statistiques réalistes.
* **Délai de réflexion aléatoire :** Préréglages *Instant*, *Rapide*, *Humain* ou *Lent*.
* **Auto-Suivant / Continuer :** Passe automatiquement les tiroirs de correction et les écrans de fin de série.
* **Mode Farm :** Arrêt automatique après un nombre défini de séries ou de minutes.

### 🎨 Interface UI Aurora
* Fenêtre déplaçable, redimensionnable librement par les bords et les coins, transparence ajustable et mode réduit en pilule flottante.

---

## 📸 Aperçu de l'interface

| Moteur & Modes | Timing & Anti-détection |
| :---: | :---: |
| ![Moteur](assets/moteur.png) | ![Timing](assets/timing.png) |

| Mémoire vérifiée (0 ms) | Réglages & Boss Key |
| :---: | :---: |
| ![Mémoire](assets/memoire.png) | ![Réglages](assets/reglages.png) |

---

## 🚀 Installation

### Étape 1 : Installer un gestionnaire de scripts
* **PC (Chrome, Edge, Brave, Opera GX, Firefox) :** [Tampermonkey](https://www.tampermonkey.net/) ou [Violentmonkey](https://violentmonkey.github.io/)
* **Android :** [Kiwi Browser](https://kiwibrowser.com/) ou Firefox Nightly + Tampermonkey
* **iOS / iPadOS :** [Userscripts](https://apps.apple.com/fr/app/userscripts/id1463298887) (Safari) ou [Orion Browser](https://browser.kagi.com/)

---

### Étape 2 : Installer VOLTERO (2 méthodes au choix)

#### 🌐 Méthode A — Installation automatique via Greasy Fork *(Recommandée)*
1. Ouvre la page officielle : [**VOLTERO — Projet Voltaire AIO sur Greasy Fork**](https://greasyfork.org/fr/scripts/607368-voltero-projet-voltaire-aio).
2. Clique sur le bouton vert **Installer ce script**, puis valide dans ton extension.
3. Les mises à jour se feront automatiquement.

#### 📦 Méthode B — Installation manuelle via GitHub Releases
1. Rends-toi dans la section [**Releases**](../../releases/latest) de ce dépôt et télécharge le fichier `VOLTERO_Projet_Voltaire_AIO.user.js`.
2. Ouvre le **Tableau de bord** de **Tampermonkey** (ou **Violentmonkey**).
3. **Glisse-dépose** le fichier `.user.js` directement dans la fenêtre de l'extension *(ou va dans `Utilitaires` → `Importer depuis un fichier`)*.
4. Clique sur **Installer**.

---

### Étape 3 : Configurer une clé API gratuite
1. Génère une clé API gratuite :
   * **Groq (recommandé, quasi instantané) :** [console.groq.com/keys](https://console.groq.com/keys) (format `gsk_...`)
   * **Google Gemini :** [aistudio.google.com/apikey](https://aistudio.google.com/apikey) (format `AIza...`)
2. Ouvre **Projet Voltaire**, déplie **`⚙️ IA, Double Vérif & Clés API`** dans le panneau VOLTERO.
3. Colle ta clé, clique sur **`Tester`**, puis appuie sur **`F9`** (ou active *AutoAnswer*) pour démarrer.

---

## ⌨️ Raccourcis & Contrôles

| Action | Raccourci PC | Tactile (Tablette / Mobile) |
| :--- | :---: | :---: |
| **Activer / Mettre en veille le moteur** | `F9` | Interrupteur *AutoAnswer (Master)* |
| **Mode Panique (masquer l'interface)** | `F8` | **Double-tap** dans le coin haut-gauche |

---

## ⚖️ Avertissement

Ce projet est publié à des fins éducatives et techniques (étude de manipulation du DOM React Native et intégration d'API LLM côté client). L'utilisateur est seul responsable de l'usage qu'il fait de cet outil.
