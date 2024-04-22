# OSL Algorithm
## Approach 1: Approximate-Model-based RL with Multimodal transformer model


### Decision making function:
#### Model-based RL
Input:
- Olfaction map
- Semantic goal-relevance map
- Robot experience
Output:
- Policy to reach goal.


### Goal function:
#### LLM goal relevance:
Input:
- Semantic map of the area
- Goal
Output:
- 
##### Approach 1:
- Goal-relevance score: given the list of objects to an LLM model, determine cosine distance of objects 

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


## Approach 2: Language model: DiLU.



# Experiment
## Simulation environment for building and testing navigation algorithm.
### Simulation environment
- Gazebo simulation environment

### Plume sensing
- Found airflow sensor, but not chemical sensor.

### Robot
#### Alternative 1: Turtlebot4 simulation.
Turtlebot4 has a preinstalled depth camera. 
- Run Turtlebot4 simulation in your laptop.
- Create a dockerfile for complete environment setup.

#### Alternative 2: Turtlebot3 simulation.

#### Alternative 3: Custom robot simulation.

### Simulation type
- VLM based vision-only navigation.


## Real world experiment for paper.
### Alternative 1: Use Turtlebot4.
### Alternative 2: Attach depth camera to Turtlebot3.
