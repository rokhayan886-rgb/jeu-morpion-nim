=========================================================================================================================================================================================================
                                                                     jeu Tictactoe ET Nim
=========================================================================================================================================================================================================
                                                      
   
Class Exécutable
******************

Les deux jeux contienent un class executable appelé Main.java donc en notation des package on a:Tous les classes executables commence par Main.java.
.
├── build
└── src
     └── games
         ├── factoredgames
         │   ├── AbstractGame.java
         │   ├── Main.java  (class excécutable)               
         │   ├── Nim.java
         │   └── TicTacToe.java
         │  
         ├── genericgames
         │   ├── AbstractGame.java
         │   ├── Game.java
         │   ├── Main.java  (class excécutable)
         │   ├── Nim.java
         │   └──  TicTacToe.java
         ├── nim
         │   ├── Main.java   (class excécutable)
         │   ├── Nim.java
         ├── players
         │   ├── Human.java
         │   ├── Main.java  (class excécutable)
         │   ├── NegamaxPlayer.java
         │   ├── Player.java
         │   └── RandomPlayer.java
         ├── plays
         │   └── Orchestrator.java
         └── tictactoe
            ├── Main.java   (class excécutable)
            └── TicTacToe.java



Mode d'Emploi
*************
Pour joeur le jeu, veuillez suivre ces étapes :
      - Assurez-vous d'avoir  installés un compilateur Java 11
      - Téléchargez l'archive et extrayez-la , ensuite compiler puis exécuter en fonction du jeu
      -Compilez et exécutez le jeu selon les instructions ci-dessous.
      
      			-------Pour le Jeu de Nim-----
	- Pour compiler ;  javac -d ../build/ nomDuPakage(games/nim)/*.java
	- Pour exécute ;  java -cp ../build/ nomDuPakage(games.nim).Main(Class éxecutable)
			------Pour le Jeu de Morpion-------
	- Pour compiler ;  javac -d ../build/ nomDuPakage(games/tictactoe)/*.java
	- Pour exécuter;  java -cp ../build/ nomDuPakage(games.tictactoe).Main(Class éxecutable)- Remarques

Régles à respecter en fonction du jeu;
				-------Pour le Jeu de Nim-----
    		- Assurez-vous de respecter les règles du jeu en ne retirant qu'un nombre valide d'allumettes 
    		-Si vous entrez un nombre invalide, le programme vous demandera de réessayer.
    			       -------Pour le Jeu de Morpion-----
    		- Ne saisissez pas un nombre inférieur à 0 ou strictement supérieur à 3.
    		- Sinon, le coup sera invalide et le joueur devra essayer d'autres valeurs.
    		-Il ne faut pas que les mêmes joueurs entrent les mêmes numéros de lignes et de colonnes.
    		


 
 Nous avons utiliser Un Main qui va gerer les 2 jeu tictactoe et nim pour la partie factorisation
************************************************************************************************

     - 	Pour le démarrage du jeu, nous avons décidé de demander à l'utilisateur de faire un choix entre les deux jeux. Il doit entrer uniquement les chiffres proposés. Si l'utilisateur entre un nombre 		au lieu d'un chiffre, cela casse le code. (Nous avons  faire autrement, sans risquer de casser le code, mais c'était plus difficile.)
     - Nous avons ajouter des getters pour les 2 joueur , une methode  switchplayer ainsi qu'un setter pour le joeur courrant	dans Abstract game
    		
    		
