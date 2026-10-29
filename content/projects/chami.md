+++
title = 'Chami'
icon = "fa-solid fa-robot"
description = "An interactive chameleon robot that helps children feel more at ease in hospital waiting rooms."
startDate = "2026-04-20"
endDate = "2026-07-03"
github = "https://github.com/mh1006/Chami-HRC_group5"
featured = true
+++

## Product Overview

**Chami** is an interactive chameleon robot designed specifically for pediatric waiting rooms. It features a fun color-matching game and provides responsive and engaging interaction to help young patients adjust to the often-frightening hospital environment.

Key features of Chami include:
* **Tactile Comfort:** The prototype is crafted with a soft green fabric exterior, making it comforting and inviting for children to touch.
*  **Emotional Support:** Chami uses non-verbal communication to interact with children. It changes its LED eye patterns and makes simple sounds depending on what the child says or does.
* **Playful Interaction:** Children play the game by pressing the physical buttons on Chami's body to match the colors displayed on its eyes.

![Chami](/image/Chami/Chami.jpg)

## Motivation
Hospital waiting rooms can be highly stressful environments, often characterized by long wait times, unfamiliar routines, and fear of upcoming medical procedures. This experience is especially overwhelming for young children. Although hospitals frequently provide conventional distractions such as books, coloring activities, or television screens, these options offer only passive engagement and may not be effective
in keeping a child’s attention away from their medical surroundings.
**Chami** was created to alleviate this stress. It acts as a friendly companion, providing a reassuring interactive experience, effectively diverting children's attention, relieving their anxiety, and allowing them to engage in play. 

## Behaviour Design: Why Non-Verbal?
### The Problem
Humanoid robots often set unrealistic expectations. In noisy hospital environments, speech recognition frequently fails, leaving children confused and frustrated when the robot cannot understand simple instructions.

### The Solution
Chami relies entirely on non-verbal communication. By adopting a zoomorphic chameleon design, its behavior strictly aligns with its animal form to eliminate the need for complex spoken language.

Instead of speaking, Chami communicates through intuitive, audio-visual, and physical feedback:

* Physical Movements: Expressive head gestures, such as nodding and shaking.

* Audio-Visual Cues: Simple animal sounds paired with distinct patterns and colors displayed on its LED eyes.

This non-verbal approach and the chameleon form serve as a natural metaphor for the color-matching game. It keeps the interaction highly expressive and approachable, while effectively reducing the children’s cognitive load.

## System & Hardware Design
To bring Chami to life, we integrated robust hardware within a soft, comforting fabric shell. The system relies on physical input/output channels to drive a multimodal interaction:
* Smart Perception (HuskyLens): Hidden in the mouth, the camera actively tracks children's faces. When a child approaches, Chami uses its rainbow eyes and head movements to gain attention.
* Tactile Gameplay Buttons: Placed along the chameleon's back for the color-matching game. Due to prototyping constraints and a shortage of LED matrix, we engineered a hybrid button system using a mix of LED and LCD screens. Although it is functional, this hardware inconsistency made us realize that user experience should be a priority in the next redesign.
* Natural Voice Control (Dialogflow): Instead of memorizing commands, children can talk freely. Dialogflow processes natural speech, transitioning the robot smoothly from casual greetings to gameplay.

<div style="display: flex; gap: 20px; align-items: stretch; justify-content: center; width: 100%;">
  
  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/Chami/frontView.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/Chami/frontView.jpg" alt="Vest Prototype" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px; margin-bottom: 0;">Front View</p>
  </div>

  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/Chami/sideView.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/Chami/sideView.jpg" alt="Circuit schematic" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px; margin-bottom: 0;">Side View</p>
  </div>

</div>

### Dual-Purpose UI: The LED Eyes
The eyes are Chami's primary communication tool, smoothly shifting between two modalities:
* Social Modality (Idle & Attracting): When resting, Chami displays a soft white blinking pattern to show it is "alive." Once the camera detects a face, the eyes instantly shift to a dynamic rainbow pattern to actively invite interaction.
* Task Modality (Gameplay): Provides clear game feedback. A correct match triggers green "happy" eyes with a rising tone, while a timeout triggers blue "sad" eyes with a dropping tone. 

<div style="display: flex; gap: 15px; align-items: stretch; justify-content: center; width: 100%;">
  
  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/Chami/eyesGreen.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/Chami/eyesGreen.jpg" alt="Happy Green Eyes" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px; margin-bottom: 0;">Happy (Green)</p>
  </div>

  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/Chami/eyesBlue.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/Chami/eyesBlue.jpg" alt="Sad Blue Eyes" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px; margin-bottom: 0;">Sad (Blue)</p>
  </div>

  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/Chami/eyesRainbow.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/Chami/eyesRainbow.jpg" alt="Attracting Rainbow Eyes" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px; margin-bottom: 0;">Attracting (Rainbow)</p>
  </div>

  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/Chami/eyesIdle.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/Chami/eyesIdle.jpg" alt="Idle Eyes" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px; margin-bottom: 0;">Idle</p>
  </div>

</div>

## User Feedback

While we couldn't bring Chami to a real pediatric ward during this short course project, our final exhibition served as a valuable testing ground. Users who interacted with Chami provided consistent and insightful feedback, giving us crucial qualitative observations on how people naturally engage with the robot.

*   **High User Acceptance:** The soft, green textile exterior and non-anthropomorphic chameleon design successfully managed user expectations. Users naturally interacted with Chami using gentle, baby-oriented language, proving the approachable design really worked.
*   **Lifelike Presence:** The combination of face-tracking and idle head movements, Chami felt genuinely alive rather than just programmed. This simple illusion of awareness naturally grabbed people's attention and drew them in.
*   **Clear Emotional Affordances:** By pairing expressive LED eye animations with non-verbal sounds, the multi-modal feedback made Chami’s internal states instantly recognizable. Users noted that the "happy" green or "sad" blue eyes provided clear feedback, and many were motivated to win the color game simply to "make the chameleon happy".

### Key Learnings & Future Iterations

While the core interaction was successful, the exhibition highlighted two valuable areas for future improvement:

* **Visual Consistency:** Due to hardware constraints, the prototype used mismatched button components (LCD and LED matrices), which caused slight confusion. Future iterations will use visually consistent buttons to clearly indicate their shared function.
* **Guiding User Attention:** Because the lifelike head movements were so engaging, users naturally focused entirely on Chami's face and occasionally missed the start of the game on its body. To solve this, the next iteration will program Chami to look at its buttons and flash them in sequence to guide the user's attention before the game begins.

Despite these minor prototype constraints, Chami proved that a thoughtfully designed, non-verbal companion can effectively reduce anxiety and offer comforting companionship to children in hospitals.

---

## Tech Stack

### **Hardware**
* **Controller**: Arduino UNO.
* **Sensor**: HuskyLens.
* **Component**: LCD, LED Matrix, buttons, Servo Motors, MP3 Module & Speaker.

### **Software**
* **Dialogue Management:** DialogFlow
* **Audio & Communication:** Semantic Free Utterance sound design, PC-Arduino Serial Communication.

---

## My Contributions

* **External Design:** Used soft textiles to create the chameleon exterior.
* **Physical Interface Design:** Designed the tangible interaction buttons on the robot's body.
* **Game Logic / Coding:** Linked the physical button inputs with the color-matching game.

---

## Team & Acknowledgments

* **Team Members**: **Ming-Hua Hsieh**, Amina Chairulina, Jada van der Heijden, Luit Meinen
* **Supervisor**: Sebastian Schneider
* **Institution**: University of Twente (UT), Enschede, the Netherlands