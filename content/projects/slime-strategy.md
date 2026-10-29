+++
title = "Slime Strategy"
icon = "fa-solid fa-chess-knight"
description = "Seize Strategy Moments in Your Hectic Life!"
startDate = "2022-11-01"
endDate = "2023-01-01"
github = "https://github.com/mh1006/Slime-Strategy"
demo = "https://www.youtube.com/watch?si=kldGSsNg9DvH3vXI&v=2sHQX9ODHoI&feature=youtu.be"
+++

## Product Overview
Many strategy games on the market either require significant time investment or are overly simplistic. As a result, people with limited time often choose other game genres for relaxation, leading them to avoid strategy games altogether.

**Slime Strategy** is a strategy game that combines a compelling storyline with easy accessibility, allowing players to learn the game mechanics in just 5 minutes and complete it within a total playtime of 30 minutes.

---

## Concept
**Slime Strategy** blends exploration and strategy, telling the story of slime villagers who want to steal the human treasure for their slime elders.
Players must create strategies to defeat humans and secure the treasure.

<div style="display: flex; justify-content: center; text-align: center; gap: 5px; flex-wrap: wrap; margin-top: 20px;">
  
  <div style="flex:0 1 160px; display: flex; flex-direction: column; align-items: center;">
    <div style="background: white; width: 100px; height: 100px; border-radius: 12px; display: flex; align-items: center; justify-content: center; margin-bottom: 15px; border: none;">
      <img src="/image/SlimeStrategy/game-plan.png" style="width: 70px; border: none !important; outline: none !important; box-shadow: none !important;">
    </div>
    <p style="font-size: 0.9em; color: #bbbbbb; margin: 0; line-height: 1.4;">Exploration</p>
  </div>

  <div style="0 1 160px; display: flex; flex-direction: column; align-items: center;">
    <div style="background: transparent; width: 100px; height: 100px; border-radius: 12px; display: flex; align-items: center; justify-content: center; margin-bottom: 15px; border: none;">
      <img src="/image/SlimeStrategy/add.png" style="width: 55px; border: none !important; outline: none !important; box-shadow: none !important;">
    </div>
  </div>

  <div style="flex:0 1 160px; display: flex; flex-direction: column; align-items: center;">
    <div style="background: white; width: 100px; height: 100px; border-radius: 12px; display: flex; align-items: center; justify-content: center; margin-bottom: 15px; border: none;">
      <img src="/image/SlimeStrategy/chess.png" style="width: 70px; border: none !important; outline: none !important; box-shadow: none !important;">
    </div>
    <p style="font-size: 0.9em; color: #bbbbbb; margin: 0; line-height: 1.4;">Strategy</p>
  </div>

</div>

## Design Goal


<div style="display: flex; justify-content: space-around; text-align: center; gap: 20px; flex-wrap: wrap; margin-top: 30px;">
  
  <div class="hover-float-item" style="flex: 1; min-width: 200px; display: flex; flex-direction: column; align-items: center; transition: transform 0.3s ease;">
    <div style="background: white; width: 100px; height: 100px; border-radius: 50%; display: flex; align-items: center; justify-content: center; margin-bottom: 15px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border: none;">
      <img src="/image/SlimeStrategy/clock.png" style="width: 50px; filter: brightness(0); border: none; outline: none; box-shadow: none;">
    </div>
    <h3 style="font-weight: bold; margin-bottom: 8px;">Short Playtime</h3>
    <p style="font-size: 0.9em; opacity: 0.7;">Completing all levels takes only 30 minutes.</p>
  </div>

  <div class="hover-float-item" style="flex: 1; min-width: 200px; display: flex; flex-direction: column; align-items: center; transition: transform 0.3s ease;">
    <div style="background: white; width: 100px; height: 100px; border-radius: 50%; display: flex; align-items: center; justify-content: center; margin-bottom: 15px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border: none;">
      <img src="/image/SlimeStrategy/relax.png" style="width: 50px; filter: brightness(0); border: none; outline: none; box-shadow: none;">
    </div>
    <h3 style="font-weight: bold; margin-bottom: 8px;">Simple Controls</h3>
    <p style="font-size: 0.9em; opacity: 0.7;">Easy to pick up and play.</p>
  </div>

  <div class="hover-float-item" style="flex: 1; min-width: 200px; display: flex; flex-direction: column; align-items: center; transition: transform 0.3s ease;">
    <div style="background: white; width: 100px; height: 100px; border-radius: 50%; display: flex; align-items: center; justify-content: center; margin-bottom: 15px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); border: none;">
      <img src="/image/SlimeStrategy/human-brain.png" style="width: 50px; filter: brightness(0); border: none; outline: none; box-shadow: none;">
    </div>
    <h3 style="font-weight: bold; margin-bottom: 8px;">Challenging Gameplay</h3>
    <p style="font-size: 0.9em; opacity: 0.7;">Requires strategic thinking and skills.</p>
  </div>

</div>

<style>
  /* 處理滑鼠移上去的微微浮起效果 */
  .hover-float-item:hover {
    transform: translateY(-10px);
  }
  /* 強制移除圖片可能產生的任何預設邊框 */
  .hover-float-item img {
    border: none !important;
    outline: none !important;
    box-shadow: none !important;
  }
</style>

## Sketch

### 1. Gameplay Flow
Players explore within the storyline and encounter enemies to battle during their journey.
<div style="display: flex; justify-content: center; margin: 40px 0;">
    <img src="/image/SlimeStrategy/gameplayFlow.png" 
         style="max-width: 100%; height: 130px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" 
         alt="Gameplay Flow">
</div>


### 2. Blockers Design


<div style="display: flex; gap: 20px; flex-wrap: wrap; align-items: stretch; margin: 40px 0; color: #000;">

  <div style="flex: 2; min-width: 300px; display: flex; flex-direction: column;">
    <div style="width: 100%; aspect-ratio: 2 / 1.2; overflow: hidden; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/blockerType.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Blockers Design">
    </div>
      <h3 style="margin: 15px 0 10px 0;">Type of Blockers</h3>
      <p style="margin: 0; font-size: 0.95em; line-height: 1.6;">We considered two ways to present obstacles in this game and ultimately chose the first option.</p>
  </div>

  <div style="flex: 1; min-width: 200px; display: flex; flex-direction: column;">
    <div style="width: 100%; aspect-ratio: 1 / 1.2; overflow: hidden; border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/blockerSimulation.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Gameplay Flow">
    </div>
    <h3 style="margin: 15px 0 10px 0;">Gameplay Flow</h3>
    <p style="margin: 0; font-size: 0.95em; line-height: 1.6;">We used a physical board to position blockers and mapped these placements into the game, creating levels with increasing complexity.</p>
  </div>

</div>

### 3. Illustrations of the User Interface
![Product](/image/SlimeStrategy/UISketch.png)

## Final Design

### Exploration 
<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 40px 0; text-align: left;">
  
  <div style="flex: 1; min-width: 150px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/explorationFinal1.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Exploration">
    </div>
    <h4 style="margin: 0 0 10px 0;">Exploration Overview</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">The exploration phase presents the story in a narrative format, allowing the player to travel the game world and unravel the plot.</p>
  </div>

  <div style="flex: 1; min-width: 150px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/explorationFinal2.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Battle Materials">
    </div>
    <h4 style="margin: 0 0 10px 0;">Collect Battle Materials</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">Player can collect materials, which can alter battle values.</p>
  </div>

  <div style="flex: 1; min-width: 150px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/explorationFinal3.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Hidden Enemy">
    </div>
    <h4 style="margin: 0 0 10px 0;">Hidden Enemy Encounters</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">Finding hidden enemies starts the strategy game phase.</p>
  </div>

</div>

### Strategy 
<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 40px 0; text-align: left;">
  
  <div style="flex: 1; min-width: 150px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/strategyFinal1.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Exploration">
    </div>
    <h4 style="margin: 0 0 10px 0;">Strategy Overview</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">The objective in the strategy part of the game is to achieve victory by defeating all enemies.</p>
  </div>

  <div style="flex: 1; min-width: 150px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/strategyFinal2.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Battle Materials">
    </div>
    <h4 style="margin: 0 0 10px 0;">Player's Turn</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">When the action is completed, press 'NEXT TURN' to end the player's turn.</p>
  </div>

  <div style="flex: 1; min-width: 150px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/strategyFinal3.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Hidden Enemy">
    </div>
    <h4 style="margin: 0 0 10px 0;">Enemy's Turn</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">The enemy (computer) will take their turn next.</p>
  </div>

</div>

#### Character’s Design 
<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 40px 0; text-align: left; color: #000;">
  
  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/initialValue.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Exploration">
    </div>
    <h4 style="margin: 0 0 10px 0;  text-align: center;">Each character’s  initial value</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5; text-align: center;">Damage = Attack - Defense</p>
  </div>

  <div style="flex: 3; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/attributeAdjustment.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Battle Materials">
    </div>
    <h4 style="margin: 0 0 10px 0;">Slime Attribute Adjustment</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">Elements collected during exploration can be used to change the battle attribute of the slimes, influencing relevant stats.</p>
  </div>
</div>

#### Detailed Design 

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 40px 0; text-align: left; color: #000;">
  
  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/interfaceOverview.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Exploration">
    </div>
    <h4 style="margin: 0 0 10px 0;">Interface Overview</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">Players can hover the mouse over each character to view specific information. Collected elements from the exploration phase are displayed at the bottom of the screen.</p>
  </div>

  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/gameEnded.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Battle Materials">
    </div>
    <h4 style="margin: 0 0 10px 0;">Game Ended</h4>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">The game will end after defeating the last enemy or when the final slime is defeated.</p>
  </div>
</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 40px 0; text-align: left; color: #000;">
  
  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/victory.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Exploration">
    </div>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5; text-align: center;">Victory will continue the player's exploration journey.</p>
  </div>

  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/defeated.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Battle Materials">
    </div>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5; text-align: center;">If defeated, the level will restart.</p>
  </div>
</div>

### UI Design
The game menu provides an overview to help players learn about the game.

<div style="display: flex; justify-content: center; margin: 40px 0;">
    <img src="/image/SlimeStrategy/menu.png" 
         style="max-width: 100%; height: 250px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" 
         alt="Gameplay Flow">
</div>

#### 1. Introduction on game controls and mechanics.
<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 40px 0; text-align: left; color: #000;">
  
  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/menu2a.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Exploration">
    </div>
  </div>

  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/menu2b.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Battle Materials">
    </div>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5; text-align: center;">Icons were designed to be animated, making their functions easier to understand.</p>
  </div>
</div>

#### 2. Display character and element parameters.

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 40px 0; text-align: left; color: #000;">
  
  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/menu3a.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Exploration">
    </div>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">Icons and text feature bold color contrasts for quick element distinction.</p>
  </div>

  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/menu3b.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Battle Materials">
    </div>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5;">A folder-shaped design simulates category flipping, with added text, images, and progress bars for clearer information.</p>
  </div>
</div>

###### A
<div style="display: flex; gap: 10px; flex-wrap: wrap; margin: 40px 0;">
  
  <div style="flex: 1; min-width: 150px;">
    <a href="/image/SlimeStrategy/menu3b1.png" data-fancybox="gallery">
      <img src="/image/SlimeStrategy/menu3b1.png" style="width: 100%; aspect-ratio: 4/3; object-fit: cover; border-radius: 8px; display: block;" alt="Image 1">
    </a>
  </div>

  <div style="flex: 1; min-width: 150px;">
    <a href="/image/SlimeStrategy/menu3b2.png" data-fancybox="gallery">
      <img src="/image/SlimeStrategy/menu3b2.png" style="width: 100%; aspect-ratio: 4/3; object-fit: cover; border-radius: 8px; display: block;" alt="Image 2">
    </a>
  </div>

  <div style="flex: 1; min-width: 150px;">
    <a href="/image/SlimeStrategy/menu3b3.png" data-fancybox="gallery">
      <img src="/image/SlimeStrategy/menu3b3.png" style="width: 100%; aspect-ratio: 4/3; object-fit: cover; border-radius: 8px; display: block;" alt="Image 3">
    </a>
  </div>

  <div style="flex: 1; min-width: 150px;">
    <a href="/image/SlimeStrategy/menu3b.png" data-fancybox="gallery">
      <img src="/image/SlimeStrategy/menu3b4.png" style="width: 100%; aspect-ratio: 4/3; object-fit: cover; border-radius: 8px; display: block;" alt="Image 4">
    </a>
  </div>

</div>

#### 3. Acknowledgment of team members and assets used in the game.

<div style="display: flex; justify-content: center; margin: 40px 0;">
    <img src="/image/SlimeStrategy/menu4.png" 
         style="max-width: 100%; height: 250px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" 
         alt="Gameplay Flow">
</div>

### Core Gameplay

<div style="display: flex; justify-content: center; margin: 40px 0;">
    <img src="/image/SlimeStrategy/startMenu.png" 
         style="max-width: 100%; height: 250px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" 
         alt="Gameplay Flow">
</div>

##### Exploration Mode Mechanics
During the exploration phase, players navigate the environment using **keyboard** controls to discover resources and progress through the story.

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 40px 0; text-align: left; color: #000;">
  
  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/start1.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Exploration">
    </div>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5; text-align: center;">Walk around to interact with characters</p>
  </div>

  <div style="flex: 1; min-width: 250px;">
    <div style="width: 100%; overflow: hidden; border-radius: 8px; margin-bottom: 15px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);">
      <img src="/image/SlimeStrategy/start2.png" style="width: 100%; height: 100%; object-fit: cover;" alt="Battle Materials">
    </div>
    <p style="margin: 0; font-size: 0.9em; line-height: 1.5; text-align: center;">Dialogue with characters</p>
  </div>
</div>

##### Strategy Mode Mechanics
Once the battle is triggered, the game transitions into a Turn-based Tactical Grid system where positioning and resource management are key to victory.

![Product](/image/SlimeStrategy/startStrategy.png)

## User testing

### Participants
* Total: 8 people
* Age range: 22 to 25 years old

### Testing Process
* Asked them to play the game without any explanations.
* Interview.

<div style="display: flex; justify-content: center; margin: 40px 0;">
    <img src="/image/SlimeStrategy/usabilityTest.png" 
         style="max-width: 100%;  border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" 
         alt="Gameplay Flow">
</div>

Players expressed a positive attitude after playing the game. 
Following are their ratings and feedback:
<div style="display: flex; justify-content: center; margin: 40px 0;">
    <img src="/image/SlimeStrategy/rate.png" 
         style="max-width: 100%;  border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" 
         alt="Gameplay Flow">
</div>

### What Worked Well
1. **Game Length and Fun**</br>
The game length is well-balanced, and the storyline is engaging.

2. **Appealing to a wide audience**</br>
The main characters are designed to be cute and appealing, making the game suitable for players of all ages and genders. 

3. **Smooth Controls**</br>
The gameplay experience is fluid and smooth.

4. **Appropriate Difficulty Level**</br>
The game offers a satisfying level of difficulty, giving players a sense of achievement during the challenges.

### What Could Be Enhanced (Severity: ☆)
1. **Improving Operational Instructions ☆☆☆☆**
* New players may not always read the instructions. 
* Display gameplay guidelines or pop-up hints with movement and attack rules before starting a new mode.

2. **Clear Action Indicators for Characters ☆☆☆**
* Players may forget which characters they’ve used when handling multiple characters.
* Make clear markers indicating which characters have completed their actions

3. **Hover Tips for Element ☆**
* The effects of using element are difficult to remember.
* When hovering over elements at the bottom, show the relevant information for each element.

4. **Color Contrast of Map Grids ☆**
* In some levels, the color of the grids is too close to the map's background, affecting visual clarity. 
* Increase the contrast between the two.

5. **Explanation of  Parameters ☆☆**
* Players might initially be unclear about the meaning of certain  parameters.
* Add explanations for each parameter, clarifying their meanings and effects.

---

## Tech Stack

* **Engine**: Unity 2021
* **Language**: C#
* **Tools**: Visual Studio, Git

---


## Contribution
### Individual Responsibilities
* **Frontend development (UI Design)**: Responsible for the overall interface layout, information architecture, and implementing character stat displays.


### Collaborative Responsibilities
*	Concept / Script Development: Brainstorming game themes and writing narrative dialogues.
*	Game Testing: Iterative testing and balancing gameplay mechanics.

---

## Team & Acknowledgments
This project was ranked **1st** out of 12 groups in the Introduction to Video Game Making course.

* **Team Members**: **Ming-Hua Hsieh**, Joshua, Luc, Moon(Art & Character Design), and Rihaam.
* **Institution**: Leiden University, the Netherlands.