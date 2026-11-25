<div align="center">

# ⚡ VOLTERO — Projet Voltaire AIO

**Suite d'assistance & d'automatisation intelligente pour Projet Voltaire (PC & Tablette)**

![Version](https://img.shields.io/badge/version-18.0-a855f7?style=for-the-badge)
![UI](https://img.shields.io/badge/UI-Aurora_Cyber_Glass-6366f1?style=for-the-badge)
![Providers](https://img.shields.io/badge/IA-Groq_%2B_Gemini-10b981?style=for-the-badge)
![Userscript](https://img.shields.io/badge/Userscript-Tampermonkey_%7C_Violentmonkey-f59e0b?style=for-the-badge)

</div>

---

## ✨ Présentation

**VOLTERO** est un userscript moderne doté d'une interface flottante **Aurora Cyber Glass** redimensionnable et déplaçable, conçu pour accompagner et automatiser l'apprentissage sur la plateforme **Projet Voltaire** (`apprentissage.appli1.projet-voltaire.fr`).

Il combine une **mémoire locale auto-apprenante** (0 latence, 0 token consommé sur les exercices déjà validés) et un **moteur IA multi-fournisseurs** (**Groq** + **Google Gemini**) avec rotation automatique des clés API et règles grammaticales intégrées.

---

## 🚀 Fonctionnalités clés

### 🧠 Moteur IA & Mémoire Vérifiée
- **Tous types d'exercices supportés :** Vocabulaire (Expression), Orthographe (détection de faute dans une phrase & QCM) et **Tableaux Cliquer / Déposer** (tri géométrique avec filtrage des emplacements fantômes React Native Web et validation automatique).
- **Mémoire auto-apprenante (0 token) :** Enregistre uniquement les réponses validées en vert par Projet Voltaire (`VOCAB`, `EXO`, `TABLEAU`) avec moteur de recherche intégré et suppression sélective.
- **Pool Multi-API & Rotation automatique :** Gérez un nombre illimité de clés **Groq** (`gsk_...`) et **Google AI Studio / Gemini** (`AIza...`), testez leur latence et leurs quotas restants en un clic, et basculez automatiquement en cas de limite `429`.
- **Auto-Scan des modèles :** Synchronisation dynamique de la liste des modèles disponibles directement depuis les endpoints Groq et Gemini.
- **Double vérification IA :** Option de seconde passe indépendante pour sécuriser les cas ambigus.

### 🎯 4 Modes d'Assistance
| Mode | Comportement |
| :--- | :--- |
| **Auto** | Résout l'exercice, clique la réponse et valide automatiquement. |
| **Vert** | Surligne la bonne réponse ou la colonne cible en vert sans cliquer. |
| **1..6** | Affiche discrètement l'index de la bonne réponse en bas à gauche de l'écran *(Vocabulaire)*. |
| **Boîte** | Affiche uniquement la solution dans le HUD de la fenêtre VOLTERO. |

### ⏱️ Furtivité, Timing & Mode Farm
- **Délai de réflexion humain :** Temps d'attente aléatoire configurable (`Instant`, `Rapide`, `Humain`, `Lent` ou curseur libre).
- **Taux de réussite ajustable :** Simule un taux d'erreur naturel (`0 %` à `100 %`).
- **Auto-Suivant / Continuer :** Enchaîne automatiquement les tiroirs de correction et écrans de fin de série.
- **Arrêt Automatique (Farm) :** Stoppe automatiquement le moteur après un nombre défini de séries ou de minutes.

---

## 📸 Aperçu de l'interface

| Onglet **Moteur** | Onglet **Timing** |
| :---: | :---: |
| ![Onglet Moteur](assets/moteur.png) | ![Onglet Timing](assets/timing.png) |
| **Onglet Mémoire** | **Onglet Réglages** |
| ![Onglet Mémoire](assets/memoire.png) | ![Onglet Réglages](assets/reglages.png) |

---

## 🛠️ Installation

1. **Installer un gestionnaire de userscripts** sur votre navigateur :
   - **PC (Chrome / Edge / Brave / Firefox) :** [Tampermonkey](https://www.tampermonkey.net/) ou [Violentmonkey](https://violentmonkey.github.io/)
   - **iPad / iPhone (Safari) :** [Userscripts](https://apps.apple.com/app/userscripts/id1463298887) ou Tampermonkey
   - **Android :** Kiwi Browser / Firefox + Tampermonkey
2. **Importer le script :**
   - Créez un nouveau script dans votre extension et collez le contenu de [`voltero.user.js`](./voltero.user.js), puis enregistrez (`Ctrl + S`).
3. **Ajouter une clé API gratuite :**
   - Ouvrez Projet Voltaire, dépliez **`⚙️ IA, Double Vérif & Clés API`** dans l'onglet **Moteur**.
   - Collez une clé gratuite obtenue sur [Groq Console](https://console.groq.com/keys) (`gsk_...`) ou [Google AI Studio](https://aistudio.google.com/apikey) (`AIza...`), puis cliquez sur **`⚡ Tout tester`**.

---

## ⌨️ Raccourcis & Gestes

| Raccourci / Geste | Action |
| :--- | :--- |
| **`F9`** | Activer / Mettre en veille **AutoAnswer (Master)** |
| **`F8`** | **Mode Panique (Boss Key)** — masque instantanément l'interface et coupe le bot |
| **Double-tap coin haut-gauche** | Active / désactive le **Mode Panique** sur tablette & tactile |
| **Glisser l'en-tête / bords** | Déplacer ou redimensionner librement la fenêtre |

---

## ⚠️ Avertissement

Ce projet est publié uniquement à des fins éducatives et de recherche sur l'automatisation web et l'intégration d'API LLM. Utilisez-le de manière responsable et dans le respect des conditions d'utilisation de la plateforme concernée.
