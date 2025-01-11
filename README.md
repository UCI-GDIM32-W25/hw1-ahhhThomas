[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MjLLqDcN)
# HW1
## W1L2 In-Class Activity

1. How would you describe this game world in objects?  
      a. Flat-colored background  
      b. Player with bunny sprite  
      c. Plants  
      d. UI tracking number of seeds remaining + number of seeds planted  
2. What attributes and actions do these objects have?  
      a. Player  
   		&emsp;i. Sprite (bunny)    
           &emsp;ii. Movement (WASD)  
          &emsp;iii. Planting (Spacebar)  
                  &emsp;&emsp;1. Sprite (plant)  
                  &emsp;&emsp;2. Spawning at character location  
      b. UI  
            &emsp;i. 2 text boxes  
           &emsp;ii. Based on seeds remaining and seeds planted  
4. How do these objects act on or affect each other?  
      a. Player movement will affect where the player is on the map  
            &emsp;i. Map is not bounded  
      b. Plant a seed at the player’s location when the space key is hit  
            &emsp;i. Condition: player has seeds remaining to plant  
           &emsp;ii. Else: cannot plant  
      c. UI is updated once a seed is placed  
            &emsp;i. +1 number of seeds planted  
           &emsp;ii. -1 number of seeds remaining  

## Devlog
Prompt: Include the HW1 break-down exercise you wrote during the Week 1 - Lecture 2 (Jan 9) in-class activity (above). If you did not attend and perform this activity, review the lecture slides and write your own plan for how you believe HW1 should be built. If your initially proposed plan turned out significantly different than the activity answers given by Prof Reid, you may want to note what was different. Then, write about how the plan you wrote in the break-down connects to the code you wrote. Cite specific class names and method names in the code and GameObjects in your Unity Scene.


Write your Devlog here!


## Open-Source Assets
If you added any other outside assets, list them here!
- [Sprout Lands sprite asset pack](https://cupnooble.itch.io/sprout-lands-asset-pack) - character and item sprites
