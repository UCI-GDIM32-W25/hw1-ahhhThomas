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

My initial proposed plan was covered all of the activity answers given by Professor Reid, although there were some differences in wording. My plan also included some notes I had while testing the HW1 build on Itch as I was under the impression that we would be building this game from scratch. For example, I noted that the background of the game was green, likely to be grass, and that the game had no boundary restrictions, meaning that the player/bunny could move off of the screen. 

There were also some differences in how we noted down conditions and updates, namely checking if a player can place seeds, updating variables when a player plants a seed when the spacebar is hit and updating the UI when it happens. I believe my style of notes helped me when I was referring back to them during programming. For example, in my Update() function, I include an if statement to catch any spacebar inputs and call my PlantSeed() function only if the player still had seeds left (in other words, _numSeedsLeft > 0) otherwise nothing will be planted. This was easy to write out in code since my notes were set up in a condition and else format--like an if-statement. 

Similarly, in my PlantSeed() function, I knew I had to instantiate a plant object and change the values of both _numSeedsLeft and _numSeedsPlanted. This is because the function is only called when spacebar is hit and if the player still has seeds remaining, meaning that a plant can be placed. Following that, the UI displaying this information must change as well, which meant that I needed to utilize the UpdateSeeds() function via _plantCountUI. 

## Open-Source Assets
If you added any other outside assets, list them here!
- [Sprout Lands sprite asset pack](https://cupnooble.itch.io/sprout-lands-asset-pack) - character and item sprites
