Readme – Jeux Tic-tac-toe Et Nim
🎮 Jeux Tic-Tac-Toe & Nim (Java)

Ce dépôt contient deux jeux classiques développés en Java : Tic-Tac-Toe (Morpion) et Nim.
Le projet met en œuvre une factorisation du code avec des classes abstraites et une architecture en packages.
📁 Structure du projet
.
├── build/
└── src/
└── games/
├── factoredgames/
│ ├── AbstractGame.java
│ ├── Main.java # Classe exécutable
│ ├── Nim.java
│ └── TicTacToe.java
│
├── genericgames/
│ ├── AbstractGame.java
│ ├── Game.java
│ ├── Main.java # Classe exécutable
│ ├── Nim.java
│ └── TicTacToe.java
│
├── nim/
│ ├── Main.java # Classe exécutable
│ └── Nim.java
│
├── players/
│ ├── Human.java
│ ├── Main.java # Classe exécutable
│ ├── NegamaxPlayer.java
│ ├── Player.java
│ └── RandomPlayer.java
│
├── plays/
│ └── Orchestrator.java
│
└── tictactoe/
├── Main.java # Classe exécutable
└── TicTacToe.java
📌 Remarque : chaque package possède sa propre classe Main.java, qui constitue le point d’entrée (classe exécutable) du jeu correspondant.

▶️ Mode d’emploi
Prérequis

Java JDK 11 ou supérieur

Un terminal (Linux, macOS ou Windows)

▶️ Lancer le jeu de Nim

Compilation :
javac -d ../build games/nim/*.java
Execution:
java -cp ../build games.nim.Main

▶️ Lancer le jeu de Tic-Tac-Toe (Morpion)

Compilation :
javac -d ../build games/tictactoe/*.java
Execution:
java -cp ../build games.tictactoe.Main

📜 Règles des jeux
🔹 Jeu de Nim

Le joueur doit retirer un nombre valide d’allumettes.

Toute saisie invalide entraîne une nouvelle demande de saisie.

🔹 Jeu de Tic-Tac-Toe (Morpion)

Les valeurs saisies doivent être comprises entre 0 et 2.

Un coup invalide oblige le joueur à recommencer.

Deux joueurs ne peuvent pas jouer sur la même case.

🧩 Factorisation et conception

Dans la partie factorisation, un seul Main permet de gérer les deux jeux (Nim et Tic-Tac-Toe).

Choix de conception :

L’utilisateur choisit le jeu à lancer via une saisie numérique.

Une saisie invalide peut interrompre le programme (une gestion plus robuste était possible mais plus complexe).

La classe AbstractGame contient :

des getters pour les deux joueurs

une méthode switchPlayer

un setter pour le joueur courant

🛠️ Technologies utilisées

Langage : Java

Paradigme : Programmation orientée objet

Concepts :

Héritage

Abstraction

Factorisation du code

Gestion de joueurs (humain / IA)

✨ Auteur

👩🏽‍💻 Rokhaya Ndiaye
Étudiante en Licence Informatique – Université de Caen Normandie

📌 Ce projet a été réalisé dans un cadre pédagogique.


