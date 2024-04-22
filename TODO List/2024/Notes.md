# Research question and hypothesis
## Research question
## Hypothesis


# OSL Algorithm

## Approach 1: Approximate-Model-based RL with Multimodal transformer model

### Vision function:
#### VLM object grounding:
Input:
- Egocentric image
- List of objects in the environment.
- Depth sensing
- Robot position

Output:
- Semantic map

### Olfaction function:
#### Infotaxis
Input: chemical and anemosensing.
Output: probable plume source in map.

### Goal-relevance of sensory input function:
#### Goal relevance for vision sensing:
Method: Given the list of objects to an LLM model, determine cosine distance of objects 
Input:
- List of objects in the area
- Goal
Output:
- Relevance of objects with goal (e.g., wall is 0, humidifier/plume is 1).

#### Goal relevance for olfactory sensing?

### Decision making function:
#### Model-based RL
Input:
- Goal-relevance map (use as initial model approximation?)
- Robot experience (update model)
Output:
- Policy to reach goal.


# Experiment
## Simulation environment for building and testing navigation algorithm.
### Simulation environment
- Gazebo simulation environment
- Gaden plume simulation

### Robot
#### Alternative 1: Turtlebot4 simulation.
Turtlebot4 has a preinstalled depth camera. 
- Run Turtlebot4 simulation in your laptop.
- Create a dockerfile for complete environment setup.

#### Alternative 2: Custom robot simulation.


## Real world experiment for paper.
### Alternative 1: Use Turtlebot4.
### Alternative 2: Attach depth camera to Turtlebot3.
