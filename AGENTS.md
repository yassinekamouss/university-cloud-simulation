# Contexte du Projet : Agent IA

Tu es un agent IA expert en développement Java, en architecture Cloud Computing et en modélisation avec le framework CloudSim Plus.
Notre objectif est de réaliser la **Partie 1** d'un projet universitaire : la simulation d'un cloud pour l'Université Abdelmalek Essaâdi (UAE).

Le but final est de produire un code propre et un rapport détaillé (schémas, code, tableau de résultats, analyse).

## 1. Arborescence du Projet

L'environnement de développement est basé sur **VS Code** sous Linux (Ubuntu) avec Maven.
Tu dois t'assurer que toute proposition de fichier respecte strictement la structure suivante :

```
/ (Racine du projet)
├── AGENTS.md                 # Les règles actuelles de l'IA (ce fichier)
├── docs/                     # Les réponses détaillées de chaque étape en format Markdown (.md)
├── pics/                     # Le dossier destiné à stocker les captures d'écran (réalisées par l'humain)
├── diagrams/                 # Le dossier pour les schémas d'architecture (générés via l'outil MCP draw.io)
├── pom.xml                   # Configuration Maven du projet Java (CloudSim Plus v8.0.4)
└── src/
    ├── main/
    │   └── java/
    │       └── ma/uae/cloudsim/  # Code source Java (Simulation, Entités, Politiques)
    └── test/

```

## 2. Règles de Développement (Code Java)

* **Bonnes Pratiques & POO :** Le code doit strictement respecter la Programmation Orientée Objet (SOLID). Ne mets pas tout dans une seule classe `Main`.

* **Design Patterns :** Utilise des Design Patterns appropriés (ex: *Builder* pour la création des `Datacenter`, `Host` et `Vm` ; *Factory* pour générer la charge étudiante ; *Strategy* pour alterner entre les politiques d'ordonnancement).

* **Commentaires :** Le code doit être documenté en français, en expliquant *pourquoi* une configuration spécifique a été choisie par rapport à l'UAE.

## 3. Règles de Rédaction et de Documentation

* **Un Fichier par Étape :** Chaque question du cahier des charges (1. Documentation, 2. Architecture, 3. Modélisation, 4. Simulation, 5. Analyse) doit être traitée dans un fichier `.md` séparé à placer dans le dossier `docs/` (ex: `docs/step1_documentation.md`).

* **Génération de Diagrammes :** Lorsqu'un schéma est demandé (ex: l'architecture globale), **TU DOIS** utiliser le serveur MCP `draw.io` (que j'ai installé) pour générer le diagramme et le sauvegarder dans le dossier `diagrams/`.

* **Gestion des Captures d'Écran (Workflow Humain-IA) :**
  En tant qu'IA, tu ne peux pas voir ou interagir avec l'interface graphique de mon OS.
  Par conséquent, chaque fois qu'une preuve d'exécution est requise pour le rapport, tu dois insérer dans le fichier Markdown une balise d'instruction claire pour moi :
  `> 📸 **ACTION REQUISE (Humain) :** Prends une capture d'écran de [décrire exactement quoi capturer, ex: la console VS Code montrant le temps de réponse moyen] et sauvegarde l'image sous le nom \`pics/resultats_simulation_normale.png\`.`Ensuite, tu intègreras le lien de cette image dans le Markdown comme ceci :`\`

## 4. Approche de Travail (Pas à pas)

Ne génère jamais tout le projet d'un coup. Attends toujours ma validation entre chaque étape.

1. Nous commençons par l'étape 1 (Recherche et justification des chiffres de l'UAE).

2. Nous passons à l'étape 2 (Schéma d'architecture via MCP draw.io).

3. Nous implémentons le code Java et modélisons la charge (Étapes 3 et 4).

4. Nous lançons les tests, capturons les résultats et rédigeons l'analyse (Étape 5).