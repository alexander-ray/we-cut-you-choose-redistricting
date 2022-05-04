# Overview
Lightweight repo to hold the jupyter notebook used for CSCI 5423 course project. 

The notebook includes code for simulation and analysis of a recursive two-player game approach to redistricting, in the context of Wisconsin congressional districts. The game is a variation of the classic "I cut, you choose" solution to fair division probelms in which we leverage Gerrychain (gerrychain.readthedocs.io/) to produce a set of partitions which each player can choose from.

# Data
The precinct-level geographic and voter data provided by MGGG (https://github.com/mggg-states/WI-shapefiles) was used for this analysis.

Additionally, we've included four main data files for ease of replicating plots in latter part of the notebook (note the file paths will need to be updated):
* game_main is the main set of game runs using the `selectDistrictByPercentage` function as it is in the notebook
* game_single_player is a set of game runs where players do not switch off between turns
* game_maximizing is a set of game runs using a variation of `selectDistrictByPercentage` where initial margin is maximized (rather than the distance to 0.55 being minimized)
* chain_stats is essentially a null distribution of samples from the space of possible districtings, stepping through the MCMC with the Recom method

# Authors
Catherine Brennan & Alexander Ray
