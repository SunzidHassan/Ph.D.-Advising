# OSL Algorithm
## Approach 1: Approximate-Model-based RL with Multimodal transformer model

Functions:
- Given model, run approximate-model-based RL navigation.
  - Use and update the model initialized by multimodal transformer model.

- Generate model for RL, given: goal-relevance map function and infotaxis function.
  - Generate goal-relevance map function, given: image, depth, position sensing.

    - Goal-relevance score: given the list of objects to an LLM model, determine cosine distance of objects 
    - **Ground goal-relevance scores in the multimodal map.**
    
  - Generate infotaxis function, given: chemical sensing, anemosensing.


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
