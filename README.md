# Open Design and Technology  
## Final Project README

> **Project Weight:** 70%  
> **Team Size:** 2 students  
> **Project Duration:** 4 weeks  
> **Class Time Available:** 6 hours per class  
> **Total Time Available:** 48 effort-hours per team  
> **Project Type:** Playful, interactive, technology-based experience

---

# Before you begin

## Fork and rename this repository
After forking this repository, rename it using the format:

`ODT-2026-TeamName`

### Example
`ODT-2026-PixelWizards`

Do not keep the default repository name.

---

# How to use this README

This file is your team’s **working project document**.

You must keep updating it throughout the 4-week build period.  
By the final review, this README should clearly show:
- your idea,
- your planning,
- your design decisions,
- your technical process,
- your build progress,
- your testing,
- your failures and changes,
- your final outcome.

## Rules
- Fill every section.
- Do not delete headings.
- If something does not apply, write `Not applicable` and explain why.
- Add images, screenshots, sketches, links, and videos wherever useful.
- Update task status and weekly logs regularly.
- Use this file as evidence of process, not only as a final report.

---

# 1. Team Identity

## 1.1 Studio / Group Name
`BananaSummer`

## 1.2 Team Members

| Name | Primary Role | Secondary Role | Strengths Brought to the Project |
|---|---|---|---|
| `Nitya` | `Coding` | `Mechanism` | `Circuit connections, breadboard wiring, debugging, soldering` |
| `Suhana` | `Fabrication` | `Mechanics` | `Physical build, Iedation + Concept sketches, Repository setup` |

## 1.3 Project Title
`MonkeyManiaMaze`

## 1.4 One-Line Pitch
`**MonkeyMania is a simple interactive maze game where you navigate using switches (arrow keys) while trying to reach the end with the same fruit you started with, despite changes along the way.**
`

## 1.5 Expanded Project Idea
In 1–2 paragraphs, explain:
- what your project is,
- what kind of playful experience it creates,
- what makes it fun, curious, engaging, strange, satisfying, competitive, or delightful,
- what technologies are involved.

**Response:**  
`MonkeyMania is a simple, forest-themed interactive maze where the player is assigned a fruit at the start; banana, blueberry, or tomato—represented through led colour. Using four directional switches, the player navigates through the maze while encountering checkpoints (“monkeys”) that change their assigned fruit (colour). The objective is to reach the end within 60 seconds while retaining the colour assigned by the maze, creating a clear rule-based system of movement, change, and outcome. The project translates a digital maze experience into a physical format, where input (switches) directly affects movement and visual output (LED feedback).

The experience is playful and engaging because it combines control with unpredictability, plus the celebratory lightshow at the end (if you win) while the player chooses their path, the changing fruit states create tension and require quick thinking. It is satisfying to successfully plan a route and finish with the correct state, especially under time pressure. The forest and monkey theme adds a narrative along with light humour, making the interaction more intuitive and memorable. Technologically, the project uses an ESP32 with MicroPython, Neopixel LED strips to form the maze paths, and a separate Neopixel to indicate the assigned colour. Due to physical constraints, multiple LED strip segments were soldered together to construct the maze layout, requiring careful circuit planning and troubleshooting, the maze becomes a sort of an illusion that the computer is instructed to follow. The structure itself is built primarily from foamboard, with paper cutouts and repurposed materials (scrap from the MSL lab) used for decoration and for a sturdy build. Tracing paper was used to to diffuse the harsh NeoPixel Light, reinforcing a hands-on, resourceful approach to both electronics and physical design.`

---

# 2. Philosophy Fit

## 2.1 Experience, Not Social Problem
This module does **not** require your project to solve a large social problem.

You are allowed to build:
- toys,
- games,
- interactive objects,
- playful machines,
- kinetic artifacts,
- humorous devices,
- strange but delightful experiences,
- things that are entertaining to use or watch.

## 2.2 What kind of experience are you creating?
Answer the following:
- What is the experience?
- What do you want the player or participant to feel?
- Why would someone want to try it again?

**Response:**  
`The experience is a short, playful, story-based arcade game where the user navigates through a forest maze while trying to retain their assigned fruit identity (colour). It combines simple controls with changing outcomes, creating a fast-paced interaction that is easy to understand but still requires attention and decision-making. The use of LEDs and colour changes turns the maze into a visually responsive system, making the experience feel active and alive, it's also heavily inspired by the mobile game 'colour switch'.

The player is meant to feel engaged, slightly challenged, and entertained. The bright colours, forest/fruit theme, and monkey theme create a childlike, lighthearted atmosphere, while the time limit and changing states add a sense of urgency and excitement. The final celebratory lightshow on victory acts as a reward, making the experience feel satisfying and complete. Someone would want to try it again because each run can play out differently depending on the path they choose and how they respond to the checkpoints, encouraging repeated attempts to “get it right” or improve their timing.`

## 2.3 Design Persona
Complete the sentence below:

> We are designing this project as if we are a small creative studio making a **[toy / game / playable object / interactive experience]** for **[children / teens / adults / classmates / exhibition visitors / mixed audience]**.

**Response:**  
`we are designing this project as if we are a small creative studio making a playable interactive game for a mixed audience, especially children and classmates.`

---

# 3. Inspiration

## 3.1 References
List what inspired the project.

| Source Type | Title / Link | What Inspired You |
|---|---|---|
| `/ App /Video Game` | `Colour Switch` | `The concept of switching colours to make it past the levels` |
| `Video Game` | `Fireboy & Watergirl` | `Simple Navigation using Arrow Keys` |
| `Arcade Game` | `Dance Revolution` | `Movement/feedback based on manually pressing or stepping on arrow keys` |

## 3.2 Original Twist
What makes your project original?

**Response:**  
`The project is original because it uses a playful narrative, monkeys throwing fruits (changing colours) to turn a simple LED maze into an engaging, story-driven experience.`

---

# 4. Project Intent

## 4.1 Core Interaction Loop
Describe the main loop of interaction.

Examples:
- press → launch → score → reset
- connect → control → observe → repeat
- turn → trigger → react → repeat
- move object → sensor detects → sound/light response → player reacts

**Response:**  
`Press Button → Navigate using Arrow Keys → Encounter Checkpoints/Targets → Colour Changes → Adjust Path → Reach End → Repeat`

## 4.2 Intended Player / Audience

| Question | Response |
|---|---|
| Who is this for? | `Mixed Audience (Classmates, Children, Exhibition visitors)` |
| Age range | `8 - 18 (enjoyable for all ages)` |
| Solo or multiplayer | `Solo` |
| Expected duration of one round | ` Under 60 Seconds` |
| What should the player feel? | `Engaged, Excited, Slightly challenged, and satisfied` |
| Is explanation required before use? | `Yes, simple instruction needed before play.` |

## 4.3 Player Journey
Describe exactly how a player will use the project.

1. **Approach:** `The player is told the goal of completing the maze within 60 seconds while keeping their assigned colour the same at the end, along with the basic rules of movement and colour change.`
2. **Start:** `The player presses any of the navigation keys to start, the system then assigns a random colour (yellow, blue or yellow), shown through the Neopixel ring.`
3. **First Action:** `After the colour has been assigned, players navigate the maze using the navigation keys.`
4. **Main Interaction:** `The player continues moving through the maze using the switches, encountering checkpoints (“monkeys”) that change their fruit/colour.`
5. **System Response:** `The LEDs update instantly to show movement and any change in fruit/colour, providing real-time visual feedback.`
6. **Win / Lose / End Condition:** `The round ends when the player reaches the exit; they win if their fruit matches the starting one within 60 seconds, rewarding them with a short lightshow, and lose if it does not or if time runs out (it flashes red).`
7. **Reset:** `The player can press any navigation key to restart/reset the game post-end-of-round.`

## 4.4 Rules of Play
If your project is a game, list the rules clearly.

- `The player is assigned a random fruit/colour (banana, blueberry, or tomato) at the start.`
- `The player must navigate the maze using the directional switches.`
- `There are 5 checkpoints in the maze that change the player’s fruit/colour.`
- `The player must reach the end within 60 seconds.`
- `To win, the player must finish the maze with the same colour they started with.`
- `If the colour does not match or time runs out, the player loses.`
- `The player can choose any path through the maze but cannot avoid all checkpoints`

---

# 5. Definition of Success

## 5.1 Definition of “Playable”
Your project will be considered complete only if these conditions are met.

- [ ] `The player can navigate the maze using all four directional switches reliably`
- [ ] `The system correctly assigns a starting fruit and displays it through LED colour`
- [ ] `All checkpoints successfully change the player’s fruit/colour when triggered`
- [ ] `The LEDs provide clear, real-time feedback during movement and interaction, and movement can be back, forth, left and right wherever possible.`
- [ ] `The player can reach the end and the system correctly determines win/lose conditions`
- [ ] `The full interaction (start → navigate → end → reset) works smoothly without errors`
- [ ] `The game can be replayed multiple times with consistent behaviour`

## 5.2 Minimum Viable Version
What is the smallest version of this project that still delivers the core experience?

**Response:**  
`The smallest version of this project would include a simplified maze with basic navigation using the four directional switches, a starting colour assignment shown through a single LED or small LED segment, and at least one checkpoint that changes the player’s fruit to a randomised colour, which the player is required to pass through multiple times. The player should still be able to move from start to end and experience the core idea of maintaining their original colour despite a change along the way. This version delivers the core experience of navigation + state change + goal, even without full decoration, multiple checkpoints, or complex visuals.`

## 5.3 Stretch Features
What features are nice to have but not essential?

- `Monkey/fruit themed elements`
- `Neopixel spinny animation for colour assinging.`
- `Lightshow at the end of the maze.`

---

# 6. System Overview

## 6.1 Project Type
Check all that apply.

- [✓] Electronics-based
- [ ] Mechanical
- [ ] Sensor-based
- [ ] App-connected
- [ ] Motorized
- [✓] Sound-based
- [✓] Light-based
- [ ] Screen/UI-based
- [✓] Fabricated structure
- [✓] Game logic based
- [✓] Installation / tabletop experience
- [ ] Other: `[Write here]`

## 6.2 High-Level System Description
Explain how the system works in simple terms.

Include:
- input,
- processing,
- output,
- physical structure,
- app interaction if any.

**Response:**  
`Input: The player uses four directional switches (up, down, left, right) to navigate through the maze.
Processing: An ESP32 running micropython processes the input, tracks the player’s position, assigns a starting colour, and updates the player’s state when checkpoints/targets are triggered.
Output: Neopixel LED strips light up to show the maze path and movement, while colour changes indicate the player’s current maze colour. An additional neopixel is used to display the assigned colour/fruit clearly. There is a short light show at the end, depending on your win or loss.
Physical Structure: The maze is built using foamboard, with LED strips arranged as paths. Multiple LED segments are soldered together to form a path for the maze, and a layer of foamboard with the maze path cutout is lined with tracing sheets to disperse the light (LED strips and NeoPixel). Paper cutouts and reused materials (wooden scraps for height) are used for decoration/build/strength.
App Interaction: There is no external app; the entire interaction is physical and self-contained.`

## 6.3 Input / Output Map

| System Part | Type | What It Does |
|---|---|---|
| `Navigational Switches (up, down, left & right)` | Input | `Allow the player to navigate through the maze by sending movement commands.` |
| `ESP32` | Processing | `Receives input, tracks position, assigns and updates colours, and controls LED output + Final light show.` |
| `LED Strips + Neopixel ring` | Output | `Display the maze path, player movement, and current fruit through colour changes.` |

---

# 7. Sketches and Visual Planning

## 7.1 Concept Sketch
Add an early sketch of the full idea.

**Insert image below:**  
`<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/5497908b-0d5b-498d-9bad-2029eac7c68d" />`
<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/ace0bfb4-2878-4ea7-8326-0f6bd09bee44" />


Example:
```md

```

## 7.2 Labeled Build Sketch
Add a sketch with labels showing:
- structure,
- electronics placement,
- user touch points,
- moving parts,
- output elements.

**Insert image below:**  
`<img width="1136" height="1600" alt="image" src="https://github.com/user-attachments/assets/ca29eae9-01c9-4ecd-b1dc-be192d202e55" />`

## 7.3 Approximate Dimensions

| Dimension | Value |
|---|---|
| Length | `21 inches` |
| Width | `21 inches` |
| Height | `3 inches` |
| Estimated weight | `2 kgs` |

---

# 8. Mechanical Planning

## 8.1 Mechanical Features
Check all that apply.

- [ ] Gears
- [ ] Pulleys
- [ ] Belt drives
- [ ] Linkages
- [ ] Hinges
- [ ] Shafts
- [ ] Springs
- [ ] Bearings
- [ ] Wheels
- [ ] Sliders
- [ ] Levers
- [✓] Not applicable

## 8.2 Mechanical Description
Describe the mechanism and what it is meant to do.

**Response:**  
`The mechanism consists of a foamboard-based maze structure that physically holds and organises the electronic components. LED strips are arranged along the maze paths and fixed onto the surface, with multiple segments soldered together to achieve the required layout. The structure guides the visual flow of the game, representing possible paths the player can take.

The directional switches act as the primary control interface, allowing the player to “move” through the maze without any physical object travelling inside it. Instead, movement is represented through changing LED positions and colours. The mechanism is designed to support a clear, stable, and interactive setup where the physical form and electronic system work together to simulate navigation.'

## 8.3 Motion Planning
If something moves, explain:
- what moves,
- what causes the movement,
- how far it moves,
- how fast it moves,
- what could go wrong.

**Response:**  
`What moves: there is no physical object moving; The “movement” is the player navigating through the maze using directional switches, and the LED lights updating to represent position and state.
What causes the movement: The player pressing the switches (input) causes the system to update the position in the maze.
How far it moves: Each button press moves the player one step or node in the maze path, long press to travel in a smooth line.
How fast it moves: Movement depends on how quickly the player presses the switches; the system responds almost instantly, although it's imperitive that the player reaches the final NeoPixel before a turn, otherwise movement it caught.
What could go wrong: Incorrect button input, delay or missed response from switches, faulty wiring or soldering in the LED strips, or incorrect state updates in the code could affect movement or feedback.`

## 8.4 Simulation / CAD / Animation Before Making
If your project includes mechanical motion, document the digital planning before fabrication.

| Tool Used | File / Link | What Was Tested |
|---|---|---|
| `[Not Applicable]` | `[Not Applicable]` | `[Not Applicable]` |
| `[Not Applicable]` | `[Not Applicable]` | `[Not Applicable]` |

## 8.5 Changes After Digital Testing
What changed after the CAD, animation, or simulation stage?

**Response:**  
`[Not Applicable]`

---

# 9. Electronics Planning

## 9.1 Electronics Used

| Component | Quantity | Purpose |
|---|---:|---|
| `[ESP32]` | `[1]` | `[Main controller]` |
| `[Jumper Wires]` | `[81]` | `[Connections between navigation switches, Neopixels and breadboard]` |
| `[USB Cable]` | `[1]` | `[Powers the ESP32 and maintains the serial connection to the laptop]` |
| `[Buck Converter]` | `[1]` | `[acts as a power supply - 5V approx.]` |
| `[LED Strips]` | `[22]` | `[Maze Path]` |
| `[NeoPixel Ring]` | `[1]` | `[Assigning starting colour]` |
| `[Switches]` | `[4]` | `[Navigating along the MonkeyManiaMaze path]` |
| `[Laptop/Computer]` | `[2]` | `[Runs Thonny for firmware, Troubleshooting]` |
| `[Breadboard]` | `[1]` | `[Organizes and stabilizes the wiring connections on the ESP32]` |

## 9.2 Wiring Plan
Describe the main electrical connections.

**Response:**  
`[The system consists of four individually controlled LED strips connected to an ESP32. The primary strip contains 9 LED segments soldered and is connected to GPIO 23. At key junction points along this main strip, three additional LED segments branch out: a 3-LED strip on GPIO 22, a 4-LED strip on GPIO 18, and a 5-LED strip on GPIO 5. Each segment is labeled and mapped to specific directional inputs, where LEDs either turn on (add) or turn off (subtract) based on button presses.

User input is handled through four push buttons connected to the ESP32:

Left → GPIO 27
Right → GPIO 32
Up → GPIO 12
Down → GPIO 14

A separate NeoPixel indicator (connected to GPIO 19) acts as a feedback signal and is triggered whenever any button is pressed.

All LED strips and input components are powered through a common ground rail on the breadboard, ensuring a shared reference across the circuit. A buck converter is integrated to regulate voltage supply to the LEDs and ESP32, maintaining stable operation.

The ESP32 is powered via USB, which also enables communication with a laptop. The system runs MicroPython through Thonny, where the firmware continuously polls the input pins, detects button presses based on predefined thresholds, and executes the corresponding LED behavior while also sending mapped keystroke signals to the browser.]`

## 9.3 Circuit Diagram
Insert a hand-drawn or software-made circuit diagram.

**Insert image below:**  
`<img width="1426" height="1600" alt="image" src="https://github.com/user-attachments/assets/5492cc18-a879-4a67-8c5b-9333d85d80bf" />`

## 9.4 Power Plan

| Question | Response |
|---|---|
| Power source | `USB connected to laptop` |
| Voltage required | `5V` |
| Current concerns | `Minimal, the Power supply was not able to fully light all the LED strips in full capacity, so we replaced it with a buck converter.` |
| Safety concerns | `Initially, on connecting the LEDs to the power supply, if there was any exchange between 5V and GND, it led to the power supply short-circuiting and causing a fire. ` |

---

# 10. Software Planning

## 10.1 Software Tools

| Tool / Platform | Purpose |
|---|---|
| `Thonny IDE` | `Writing, uploading and debugging the MicroPython firmware on the ESP32` |
| `MicroPython` | `[The firmware language running on the ESP32 that handles input and output]` |

## 10.2 Software Logic
Describe what the code must do.

Include:
- startup behavior,
- input handling,
- sensor reading,
- decision logic,
- output behavior,
- communication logic,
- reset behavior.

**Response:**  
`Startup behavior: When powered on, the system resets all LEDs to off, initializes the game state, and waits for the player to press any button to begin. Once a button is pressed, a spinning LED animation (neopixel ring) runs to assign a random starting fruit/colour.`
`Input handling: The system continuously reads input from four directional push buttons (up, down, left, right) using a debounce delay to prevent accidental multiple inputs.
sensor reading: there are no external sensors; the system relies entirely on button inputs as user interaction.`
`Decision logic: The code tracks the player’s position within different maze segments and branches. When the player reaches specific checkpoints, the system updates the current fruit/colour. It also checks whether the player has reached the end and compares the current fruit with the originally assigned one to determine a win or a loss.`
`Output behavior: Neopixel led strips light up to show the player’s movement through the maze and update colour based on the current fruit. The neopixel ring displays the starting colour through a spinning animation. Additional animations are triggered for win (colourful light sequence) and lose (red blinking).`
`Communication logic: There is no external communication; all processing and interaction happen within the ESP32 system.`
`Reset behavior: After a win or lose condition, the system runs the respective animation, turns all LEDs off, resets all positions and states, assigns a new random fruit, and returns to the waiting state for the next round.`


## 10.3 Code Flowchart
Insert a flowchart showing your code logic.

Suggested sequence:
- start,
- initialize,
- wait for input,
- read input,
- decision,
- trigger output,
- repeat or reset,
- error handling.

**Insert image below:**  
`<img width="386" height="579" alt="Flowchart yum" src="https://github.com/user-attachments/assets/118da215-95a1-4f3c-84d3-549944b9f351" />`

## 10.4 Pseudocode

```text
START

INITIALIZE:
    set up button inputs (up, down, left, right)
    set up neopixel strips (main + branches + spinner)
    turn all LEDs OFF
    define colour list (pink, yellow, blue)
    set game_state = "spinning"

LOOP FOREVER:

    IF game_state == "spinning":
        turn all LEDs OFF
        wait until any button is pressed
        assign random starting colour
        run spinner animation
        display assigned colour on spinner
        render maze LEDs
        set game_state = "playing"

    IF game_state == "playing":
        read button inputs (up, down, left, right)

        IF any button pressed AND debounce condition satisfied:
            update player position in maze
            (handle movement across segments and branches)

            IF player reaches checkpoint:
                change colour (cycle through colours)

            update LEDs to reflect:
                - current position
                - current colour

            IF player reaches end:
                IF current colour == assigned starting colour:
                    set game_state = "win"
                ELSE:
                    set game_state = "lose"

    IF game_state == "win":
        run win animation (multicolour sparkle)
        turn LEDs OFF
        wait briefly
        reset all variables and positions
        set game_state = "spinning"

    IF game_state == "lose":
        run lose animation (red blinking)
        turn LEDs OFF
        wait briefly
        reset all variables and positions
        set game_state = "spinning"

END LOOP
```

---

# 11. MIT App Inventor Plan

## 11.1 Is an app part of this project?
- [ ] Yes
- [✓] No

If yes, complete this section.

## 11.2 Why is the app needed?
Explain what the app adds to the experience.

Examples:
- remote control,
- score tracking,
- mode selection,
- personalization,
- triggering effects,
- displaying data.

**Response:**  
`[Not Applicable]`

## 11.3 App Features

| Feature | Purpose |
|---|---|
| `[Bluetooth connect button]` | `[Purpose]` |
| `[Score display]` | `[Purpose]` |
| `[Control button / slider / label]` | `[Purpose]` |

## 11.4 UI Mockup
Insert a sketch or screenshot of the app interface.

**Insert image below:**  
`[Upload image and link here]`

## 11.5 App Screen Flow

1. `[Step 1]`
2. `[Step 2]`
3. `[Step 3]`
4. `[Step 4]`

---

# 12. Bill of Materials

## 12.1 Full BOM

| Item | Quantity | In Kit? | Need to Buy? | Estimated Cost | Material / Spec | Why This Choice? |
|---|---:|---|---|---:|---|---|
| `[ESP32]` | `1` | `Yes` | `No` | `0` | `[Spec]` | `[Enables wireless keyboard input and touch sensing in one board]` |
| `[Jumper Wires]` | `[81]` | `[Yes]` | `[No]` | `[0]` | `[81]` | `[[connection between Neopixels, Switches and ESP32 pins]]` |
| `[FoamBoard]` | `[2]` | `[No]` | `[No]` | `[0]` | `[28 × 28 inches]` | `[Build the overall maze structure/box/structural lifts]` |
| `[A3 paper/Chart Paper/Corrogated paper]` | `[8]` | `[No]` | `[Yes]` | `[150]` | `[120/150 gsm A3/A2]` | `[Cover the foamboard, decor, structural value]` |
| `[Gluestick/Fevicol]` | `[1]` | `[No]` | `[Yes]` | `[150]` | `[120/150 gsm A3/A2]` | `[Cover the foamboard, decor, structural value]` |
| `[Buck Converter]` | `[1]` | `[No]` | `[No (borrowed)]` | `[0]` | `[N/A]` | `[Power Supply was insufficient]` |
| `[LED Strips]` | `[3 meters]` | `[No]` | `[Yes]` | `[600rs]` | `[3 meters]` | `[Maze Path]` |

## 12.2 Material Justification
Explain why you selected your main materials and components.

Examples:
- Why acrylic instead of cardboard?
- Why MDF instead of 3D print?
- Why servo instead of DC motor?
- Why bearing instead of a plain shaft hole?

**Response:**  
`[The materials and components were chosen based on availability, ease of use, and suitability for a quick interactive prototype. Foamboard was used for the structure because it is lightweight, easy to cut, we didn't use MDF since there were so many changes along the fabrication, and sturdy enough to support the LED layout, making it ideal for building the maze form without complex tools. Paper materials like chart paper and corrugated sheets were used to cover and decorate the structure, adding visual clarity and reinforcing the forest theme while also improving the overall finish.

Neopixel LED strips were selected because they allow individual control of each LED, which is essential for showing movement and colour changes within the maze. Jumper wires and basic soldering were used to connect multiple LED segments due to layout constraints, ensuring flexibility in building the maze shape. The buck converter was included to provide stable power to the LEDs, as the initial supply was insufficient, making the system more reliable. Overall, the choices prioritised flexibility and cost-effectiveness while supporting the interactive experience.]`

## 12.3 Items to Purchase Separately

| Item | Why Needed | Purchase Link | Latest Safe Date to Procure | Status |
|---|---|---|---|---|
| `[LED strips]` | `[Maze path]` | `[https://www.digikey.in/en/products/detail/sparkfun-electronics/12021/5673739]` | `[10/04/2026]` | `[Recieved` |
| `[Buck converter]` | `[supply power]` | `[https://robocraze.com/products/lm2596-dc-dc-step-down-buck-module-with-display?variant=44512742342880&country=IN&currency=INR&utm_medium=product_sync&utm_source=bing&utm_content=sag_organic&utm_campaign=sag_organic&utm_source=bing&utm_medium=ppc&utm_campaign=523565826&utm_content=_&utm_term=&campaignid=523565826&adgroupid=1327113235784461&campaign=523565826&msclkid=a81105f5a75d18d238696c1c16b21277]` | `[10/04/2026]` | `[Recieved]` |
| `[Coloured chart paper]` | `[visuals]` | `[https://www.amazon.in/Collections-Multicolor-Bright-Pastel-Drawing/dp/B0CJPZZ8L5/ref=sr_1_9?adgrpid=1312818493089728&dib=eyJ2IjoiMSJ9.uodJPqmjjgzA4T9ghJ6zbAbaJh20x2mu-MC4gJBaJ4YpiwIkxZn_WBUfE8yKq14RoQA01zBXHnXXJRMfSlV2pCE18ZG_lpF8gD7M1iccUECWSv_ybHX6ry64wSn2pq-cuDESRH2NFAMdtrpx0aIN5k0XdWsSLHEyKeNTx9DuZuol40nfHX7bfLYnqsvirJYITa2TomzsMcJpADXZvrigs1n1VswErSpNKGGgR_pOUKg-trO_p2zuO0Yt2VIih_xfWHooG129l0v0bgwXoEre_ngW043jvQC_wdR7AmCs_b4.xBBL0THSLp0qw2uh1m5UlTJR3gO1hFzgC1JbYRA3oXE&dib_tag=se&hvadid=82051414146659&hvbmt=bb&hvdev=c&hvlocphy=148579&hvnetw=o&hvqmt=b&hvtargid=kwd-82052037257254%3Aloc-90&hydadcr=7700_1981652&keywords=craft%2Bchart%2Bpaper&mcid=54f7a634cc713c1b85b283bd68d19608&msclkid=8cb564ca880b166f2b890d233a296069&nsdOptOutParam=true&qid=1776923174&sr=8-9&th=1]` | `[10/04/2026]` | `[Recieved]` |
| `[Corrugated sheet]` | `[visuals]` | `[https://www.amazon.in/Multicolour-Corrugated-Scrapbook-Decoration-Multipurpose/dp/B0FG95G44R/ref=sr_1_6?crid=1QUE74ENUY3QL&dib=eyJ2IjoiMSJ9.uHh7YZb4IUlycsNKaysb6YRTc-16CQE0nyOdZJx8A1jXwZtChNqCgO-Gg4LoIqdxaDyPxaa6VaJAhGgzU8BuGv022WeOdMgmQskZb0aeyO3KUeKuggtd2XF46R2HGRqbP-l8U_h-D_phuxR9g-ETODCZWpx3b1Edb5TQSrsY4qVguYZyXD4u-adwkVUcdeVce0V3sDAGQGW387a5ZWcT3WHz63BUjlLKkHGHE8eV_PWVMcqvvvTd-0ffQcLiI05Up4s25egEP0I51z2lFY6ei2uco1gm7OrBLGniGJuCJZM.yzSfqbDymYgIOluNfNjKSYBFf-bTqVOt2g3Oi3jiNDs&dib_tag=se&keywords=corrugated+sheet&qid=1776923209&sprefix=corrugated+she%2Caps%2C415&sr=8-6]` | `[10/04/2026]` | `[Ordered]` |

## 12.4 Budget Summary

| Budget Item | Estimated Cost |
|---|---:|
| Electronics | `[600]` |
| Mechanical parts | `[-]` |
| Fabrication materials | `[200]` |
| Purchased extras | `[125]` |
| Contingency | `[-]` |
| **Total** | `[925]` |

## 12.5 Budget Reflection
If your cost is too high, what can be simplified, removed, substituted, or shared?

**Response:**  
`[Not Applicable]`

---

# 13. Planning the Work

## 13.1 Team Working Agreement
Write how your team will work together.

Include:
- how tasks are divided,
- how decisions are made,
- how progress will be checked,
- what happens if a task is delayed,
- how documentation will be maintained.

**Response:**  
`[Our team worked by dividing responsibilities based on individual strengths while still collaborating on key decisions. suhana primarily focused on fabrication, including building the foamboard structure, assembling the maze layout, and handling visual elements and finishing. nitya focused on the technical aspects such as coding, circuit setup, soldering, and ensuring the system functioned correctly. despite this division, both members were involved in testing, troubleshooting, and refining the overall experience.

decisions were made through discussion, especially when it came to changes in the concept, layout, or system behaviour. we regularly checked progress by reviewing both the physical build and the code together, ensuring that all parts were aligned and functioning as intended. if a task was delayed, we adjusted by redistributing smaller responsibilities or working together to complete critical parts, particularly during troubleshooting stages. documentation was maintained alongside the process, with notes and images that captured changes, and final outcomes.
]`

## 13.2 Task Breakdown

| Task ID | Task | Owner | Estimated Hours | Deadline | Dependency | Status |
|---|---|---|---:|---|---|---|
| T1 | `[Finalize concept]` | `[Nitya + Suhana]` | `2` | `[05/04/26]` | `None` | `Done` |
| T2 | `[Complete BOM]` | `[Nitya + Suhana]` | `1` | `[10/04/26]` | `T1` | `Done` |
| T3 | `[Test electronics]` | `[Nitya]` | `2` | `[12/04/26]` | `T1` | `Done` |
| T4 | `[Build structure]` | `[Suhana]` | `4` | `[20/04/26]` | `T1` | `Done` |
| T5 | `[Write control code]` | `[Nitya]` | `4` | `[19/04/26]` | `T3` | `Done` |
| T6 | `[Integrate system]` | `[Suhana]` | `4` | `[20/04/26]` | `T4, T5` | `Done` |
| T7 | `[Playtest]` | `[Nitya + Suhana]` | `2` | `[20/04/26]` | `T6` | `Done` |
| T8 | `[Refine and document]` | `[Nitya + Suhana]` | `3` | `[20/04/26]` | `T7` | `Done` |

## 13.3 Responsibility Split

| Area | Main Owner | Support Owner |
|---|---|---|
| Concept and gameplay | `[Nitya + Suhana]` | `[None]` |
| Electronics | `[Nitya]` | `[Suhana]` |
| Coding | `[Nitya]` | `[Suhana]` |
| App | `[Not Applicable]` | `[Not Applicable]` |
| Mechanical build | `[Suhana]` | `[Nitya]` |
| Testing | `[Nitya + Suhana]` | `[None]` |
| Documentation | `[Suhana]` | `[Nitya]` |

---

# 14. Weekly Milestones

## 14.1 Four-Week Plan

### Week 1 — Plan and De-risk
Expected outcomes:
- [✔] Idea finalized
- [ ] Core interaction decided
- [✔] Sketches made
- [ ] BOM completed
- [✔] Purchase needs identified
- [✔] Key uncertainty identified
- [✔] Basic feasibility tested

### Week 2 — Build Subsystems
Expected outcomes:
- [✔] Electronics tests completed
- [ ] CAD / structure planning completed
- [ ] App UI started if needed
- [ ] Mechanical concept tested
- [✔] Main subsystems partially working

### Week 3 — Integrate
Expected outcomes:
- [ ] Physical body built
- [✔] Electronics integrated
- [✔] Code connected to hardware
- [ ] App connected if required
- [ ] First playable version exists

### Week 4 — Refine and Finish
Expected outcomes:
- [✔] Technical bugs reduced
- [✔] Playtesting completed
- [✔] Improvements made
- [ ] Documentation completed
- [✔] Final build ready

## 14.2 Weekly Update Log

| Week | Planned Goal | What Actually Happened | What Changed | Next Steps |
|---|---|---|---|---|
| Week 1 | `[Finalize concept and basic system plan]` | `[Decided on wall-based dance revolution]]` | `[tried to come up with a system for both hands and feet]` | `[Write here]` |
| Week 2 | `[Write here]` | `[Write here]` | `[Write here]` | `[Write here]` |
| Week 3 | `[Write here]` | `[Write here]` | `[Write here]` | `[Write here]` |
| Week 4 | `[Write here]` | `[Write here]` | `[Write here]` | `[Write here]` |

---

# 15. Risks and Unknowns

## 15.1 Risk Register

| Risk | Type | Likelihood | Impact | Mitigation Plan | Owner |
|---|---|---|---|---|---|
| `[Example: Bluetooth disconnects]` | `Technical` | `Medium` | `High` | `[Fallback interaction / simplify connection flow]` | `[Name]` |
| `[Example: Structure breaks during play]` | `Mechanical` | `Medium` | `High` | `[Reinforce joints / change material]` | `[Name]` |
| `[Risk]` | `[Technical / Material / Time / Gameplay]` | `[Low/Medium/High]` | `[Low/Medium/High]` | `[Plan]` | `[Name]` |
| `[Risk]` | `[Type]` | `[Low/Medium/High]` | `[Low/Medium/High]` | `[Plan]` | `[Name]` |

## 15.2 Biggest Unknown Right Now
What is the single biggest uncertainty in your project at this stage?

**Response:**  
`[Write here]`

---

# 16. Testing and Playtesting

## 16.1 Technical Testing Plan

| What Needs Testing | How You Will Test It | Success Condition |
|---|---|---|
| `[Bluetooth connection]` | `[Method]` | `[What counts as success?]` |
| `[Mechanism movement]` | `[Method]` | `[What counts as success?]` |
| `[Sensor behavior]` | `[Method]` | `[What counts as success?]` |
| `[App communication]` | `[Method]` | `[What counts as success?]` |

## 16.2 Playtesting Plan

| Question | How You Will Check |
|---|---|
| Do players understand what to do? | `[Method]` |
| Is the interaction satisfying? | `[Method]` |
| Do players want another turn? | `[Method]` |
| Is the challenge balanced? | `[Method]` |
| Is the response clear and immediate? | `[Method]` |

## 16.3 Testing and Debugging Log

| Date | Problem Found | Type | What You Tried | Result | Next Action |
|---|---|---|---|---|---|
| `[Date]` | `[Describe issue]` | `[Technical / Mechanical / UI / Gameplay]` | `[What you did]` | `[Worked / Partly / Failed]` | `[Next step]` |
| `[Date]` | `[Describe issue]` | `[Type]` | `[What you did]` | `[Result]` | `[Next step]` |

## 16.4 Playtesting Notes

| Tester | What They Did | What Confused Them | What They Enjoyed | What You Will Change |
|---|---|---|---|---|
| `[Peer / friend / classmate]` | `[Observation]` | `[Observation]` | `[Observation]` | `[Action]` |
| `[Peer / friend / classmate]` | `[Observation]` | `[Observation]` | `[Observation]` | `[Action]` |

---

# 17. Build Documentation

## 17.1 Fabrication Process
Describe how the project was physically made.

Include:
- cutting,
- 3D printing,
- assembly,
- fastening,
- wiring,
- finishing,
- revisions.

**Response:**  
`[the fabrication process was entirely manual and evolved throughout the project. the maze structure was built using waste foamboard, which was cut and assembled to create different layers, supported by scrap HDF wood pieces for stability. the surface was covered with chart paper for a cleaner finish, and tracing sheets were used to define the maze paths where the led strips were placed.

a major part of the process was planning and wiring the led system. we had to break the strips into 22 separate segments and manually solder them together to match the maze layout, which required careful planning of pathways before continuing the build. this wiring and soldering process took up a significant portion of the time.

for the visual elements, monkey graphics were first designed in figma, but since printing did not work out, all elements were hand-cut instead. additional detailing was done using colour pencils, and scrap paper from previous projects was repurposed for decoration. the project went through multiple revisions as the structure kept evolving, which is why flexible materials were chosen over rigid ones like mdf. finishing involved assembling all components and refining the overall look to match the theme.]`

## 17.2 Build Photos
Add photos throughout the project.

Suggested images:
- early sketch,
- prototype,
- electronics testing,
- mechanism test,
- app screenshot,
- final build.

Example:
```md

in the folders above

```

## 17.3 Version History

| Version | Date | What Changed | Why |
|---|---|---|---|
| v1 | initial stage | concept shifted from dance/twister-style game to led maze | to create a more original idea and better suit available resources |
| v2 | development stage | maze layout designed, led segments planned and soldered, basic movement and colour logic implemented | to make the system functional and solve physical constraints of led placement |
| v3 | final stage | defined a theme, spinner for colour assignment, checkpoints, and win/lose animations | to improve user experience, clarity, and overall engagement |

---

# 18. Final Outcome

## 18.1 Final Description
Describe the final version of your project.

**Response:**  
`[the final version of the project is a fully functional, forest-themed interactive maze game called monkeymania. the player navigates through the maze using four directional switches (up, down, left, right), while led strips visually represent their movement and current state. at the start, a spinning neopixel ring assigns the player a random fruit—banana, blueberry, or tomato—represented through colour. as the player moves through the maze, they encounter checkpoints that change the colour of the light, adding challenge and unpredictability.

the goal is to reach the end of the maze within 60 seconds while maintaining the original colour assigned at the start. the system provides real-time visual feedback through multiple neopixel led segments that form the maze paths, along with distinct animations for winning (multicolour light sequence) and losing (red blinking). the entire structure is built using foamboard, with paper elements used for decoration and theme, and the electronics are connected through soldered led segments and controlled by an esp32 running micropython. the final outcome is a simple but engaging interactive experience that combines physical input and output.
]`

## 18.2 What Works Well
- `[The navigation system works reliably, with each switch correctly moving the player through the maze without major input errors]`
- `[Led feedback is immediate and accurate, clearly showing both player position and colour changes at checkpoints]`
- `[The game logic functions as intended, including correct colour assignment, checkpoint-based colour switching, and accurate win/lose detection]`

## 18.3 What Still Needs Improvement
- `[The physical structure could be more compact and better integrated for stability and portability]`
- `[Visual finishing and detailing can be refined.]`
- `[The starting interaction could be clearer with a dedicated start button instead of relying on any button press]`

## 18.4 What Changed From the Original Plan
How did the project change from the initial idea?

**Response:**  
`[The project evolved significantly from the initial idea. originally, we planned to create a game inspired by dance revolution and twister, focusing more on physical movement and coordination. however, we decided to shift towards a more original and achievable concept that better suited our resources and time constraints, leading to the development of an interactive led maze.

as the idea progressed, the design became more refined and structured. the early concept of the maze was quite basic, with simple light changes at certain points and no clear theme. over time, this developed into a more cohesive experience with a forest/monkey narrative and a fruit-based colour system, making the interaction more engaging and intuitive. technically, the project also changed in terms of execution as initially, the maze layout and wiring were loosely planned, but during the building process, we had to rethink how the led strips would be segmented and soldered due to physical constraints. this led to a more modular approach, with multiple led segments connected to form the final maze. overall, the project shifted from a generic idea to a more defined, interactive system with clearer gameplay and identity.
]`

---

# 19. Reflection

## 19.1 Team Reflection
What did your team do well?  
What slowed you down?  
How well did you manage time, tasks, and responsibilities?

**Response:**  
`[We worked well by dividing tasks based on strengths and supporting each other during testing and troubleshooting. What slowed us down was resolving technical issues like wiring and soldering along with lack of availability of materials, which required multiple iterations. overall, we managed time and responsibilities effectively, adjusting tasks when needed and ensuring the project was completed with all core features working.]`

## 19.2 Technical Reflection
What did you learn about:
- electronics,
- coding,
- mechanisms,
- fabrication,
- integration?

**Response:**  
`[we learned how to work with electronics by managing multiple led strips, soldering connections, and ensuring stable power using a buck converter. in coding, we understood how to structure logic using states, handle inputs with debounce, and control neopixels for dynamic visual output.

we also learned that even without moving parts, mechanisms can be created through system logic and interaction. in fabrication, we explored building with foamboard and adapting materials to fit the soft design. Most importantly, we learned integration, how to bring together code, electronics, and physical structure into one functioning, cohesive system.]`

## 19.3 Design Reflection
What did you learn about:
- designing for play,
- delight,
- clarity,
- physical interaction,
- player understanding,
- iteration?

**Response:**  
`[we learned that play works best when rules are simple but outcomes are dynamic. Clarity comes from instant visual feedback, and delight comes from small elements like colour and theme. Physical interaction must be responsive for the system to feel reliable. using familiar ideas improves player understanding, and continuous iteration helped us refine both the concept and execution.]`

## 19.4 If You Had One More Week
What would you improve next?

**Response:**  
`[if we had one more week, we would further refine the visual finish and improve the overall structure by integrating the breadboard and electronics more seamlessly into the body of the maze, making it more compact and portable. while the current setup functions effectively, this would enhance durability and ease of handling. we would also add a dedicated start button to make the interaction even more intuitive and clearly define the beginning, also work on a small rule sheet for further clarity. 
]`

---

# 20. Final Submission Checklist

Before submission, confirm that:
- [✔] Team details are complete
- [✔] Project description is complete
- [✔] Inspiration sources are included
- [✔] Player journey is written
- [✔] Sketches are added
- [✔] BOM is complete
- [✔] Purchase list is complete
- [✔] Budget summary is complete
- [ ] Mechanical planning is documented if applicable
- [ ] App planning is documented if applicable
- [✔] Code flowchart is added
- [✔] Task breakdown is complete
- [✔] Weekly logs are updated
- [✔] Risk register is complete
- [✔] Testing log is updated
- [✔] Playtesting notes are included
- [✔] Build photos are included
- [✔] Final reflection is written

---

# 21. Suggested Repository Structure

```text
project-repo/
├── README.md
├── images/
│   ├── concept-sketch.jpg
│   ├── labeled-sketch.jpg
│   ├── circuit-diagram.jpg
│   ├── ui-mockup.jpg
│   ├── prototype-1.jpg
│   └── final-build.jpg
├── code/
│   ├── main.py
│   ├── test_code.py
│   └── notes.md
├── cad/
│   ├── models/
│   └── screenshots/
└── docs/
    ├── references.md
    └── extra-notes.md
```

---

# 22. Instructor Review

## 22.1 Proposal Approval
- [✔] Approved to proceed
- [✔] Approved with changes
- [✔] Rework required before proceeding

**Instructor comments:**  
`[Instructor fills this section]`

## 22.2 Midpoint Review
`[Instructor fills this section]`

## 22.3 Final Review Notes
`[Instructor fills this section]`
