# GroupAD README
A Monte Carlo Tree Search (MCTS) agent enhanced with heuristic-driven decision-making for the Sushi Go! environment in the TAG Framework. 

## Description
This project contains the implementation of GroupAD’s BasicMCTSPlayerv4, an advanced Monte Carlo Tree Search agent developed for the Sushi Go! framework.

It improves upon the standard BasicMCTSPlayer by introducing:

A heuristic evaluator (SushiGoHeuristicversion4) for better state estimation

A custom tree node (BasicTreeNodeXversion4) using softmax-based expansion and UCB1 exploration

Optimised rollout depth and adaptive exploration for balanced performance

## Dependencies

Before running this agent, ensure you have the following installed and configured:
Java 8 or later

Core Sushi Go! framework including:

core.AbstractGameState

core.actions.AbstractAction

players.basicMCTS.BasicMCTSPlayer

players.basicMCTS.BasicMCTSParams

players.PlayerConstants

## Installing

Clone or copy this repository into your workspace.

Maintain the following structure:

src/
  main/
    java/
      core/
      players/
        basicMCTS/
          groupADversion4/


Add the following Java files to groupADversion4/:

GroupADBasicMCTSPlayerversion4.java

BasicTreeNodeXversion4.java

SushiGoHeuristicversion4.java

Compile with:

javac -cp ./src ./src/main/java/players/basicMCTS/groupADversion4/*.java

## Executing the programme

To run the game with your agent:

Navigate to:

src/main/java/core/Game.java


Inside the public static void main(String[] args) method, locate:

ArrayList<AbstractPlayer> players = new ArrayList<>();


Uncomment the players you wish to test and comment out those you do not want to play, for example:

players.add(new GroupADBasicMCTSPlayerversion4());


Save the file and run:

java -cp ./src main.java.core.Game


Your selected agents will automatically play against each other once the programme starts.

## Help

If you encounter issues:

Ensure that all player versions (GroupADBasicMCTSPlayerversion1–4) are correctly placed under players/basicMCTS/.

Confirm that BasicMCTSParams includes a valid heuristic (SushiGoHeuristicversion4).

If compilation fails, check that your imports match your package hierarchy exactly.

## Authors

Group AD

## Licence

This project is part of the ECS7032P Coursework and intended solely for academic and educational use.
Redistribution or commercial usage is not permitted without written permission.

Abdulhafiz Altamimi — 250996968

Adnan Hussain — 240906373

Omar Debbah — 251038283

