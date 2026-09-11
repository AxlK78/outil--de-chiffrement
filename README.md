# Outil de Chiffrement de Vigenère

**Projet académique — Bachelor Cybersécurité (EPITA x École Polytechnique)**

Ce projet est un outil en ligne de commande (CLI) développé en Python. Il permet de chiffrer et déchiffrer des chaînes de caractères, des fichiers isolés, ainsi que l'intégralité des fichiers d'un répertoire en appliquant l'algorithme cryptographique de Vigenère.

Ce programme a été conçu pour illustrer l'implémentation d'un algorithme mathématique historique tout en intégrant des manipulations de bas niveau du système de fichiers (parcours récursif, processus de lecture/écriture, gestion des chemins).

## 1. Fonctionnalités Principales

- **Gestion des clés** : Création de clés pseudo-aléatoires d'une longueur paramétrable (minimum 8 caractères) ou saisie manuelle.
- **Export** : Sauvegarde automatique de la clé générée dans un fichier de sortie dédié (`cle.txt`).
- **Traitement multiniveau** :
  - **Mode interactif** : Chiffrement et déchiffrement de texte à la volée via l'entrée standard.
  - **Mode fichier** : Traitement direct du contenu d'un fichier cible avec écrasement in-place.
  - **Mode répertoire** : Parcours récursif automatisé d'un dossier pour appliquer le traitement cryptographique à l'ensemble de son arborescence.
- **Résilience** : Maintien de l'intégrité des caractères non-alphabétiques originaux (ponctuation, espaces) et gestion des exceptions liées au système de fichiers.

## 2. Environnement Technique

| Composant | Détail |
|---|---|
| Langage principal | Python 3 |
| Bibliothèques standard | `os` (interactions système, résolution de chemins absolus), `random` (génération d'entropie) |
| Scripting d'automatisation | Bash (`application.sh`) |

## 3. Déploiement et Utilisation

Le projet s'exécute nativement avec Python 3. Aucune dépendance externe (requérant `pip`) n'est nécessaire.
