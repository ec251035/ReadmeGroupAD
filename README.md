# ReadmeGroupAD
A Monte Carlo Tree Search (MCTS) agent enhanced with heuristic-driven decision-making for the Sushi Go! environment. 

# Description
This project contains the implementation of GroupAD’s BasicMCTSPlayerv4, an advanced Monte Carlo Tree Search agent developed for the Sushi Go! framework.

It improves upon the standard BasicMCTSPlayer by introducing:

A heuristic evaluator (SushiGoHeuristicversion4) for better state estimation

A custom tree node (BasicTreeNodeXversion4) using softmax-based expansion and UCB1 exploration

Optimised rollout depth and adaptive exploration for balanced performance

# Dependencies

Before running this agent, ensure you have the following installed and configured:
Java 8 or later

Core Sushi Go! framework including:

core.AbstractGameState

core.actions.AbstractAction

players.basicMCTS.BasicMCTSPlayer

players.basicMCTS.BasicMCTSParams

players.PlayerConstants

# Installing


