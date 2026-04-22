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
`[Upload image and link here]`

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
`[Upload image and link here]`

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
| `[ESP32]` | `1` | `Yes` | `No` | `0` | `[Spec]` | `[Reason]` |
| `[Item]` | `[Qty]` | `[Yes/No]` | `[Yes/No]` | `[Cost]` | `[Spec]` | `[Reason]` |
| `[Item]` | `[Qty]` | `[Yes/No]` | `[Yes/No]` | `[Cost]` | `[Spec]` | `[Reason]` |

## 12.2 Material Justification
Explain why you selected your main materials and components.

Examples:
- Why acrylic instead of cardboard?
- Why MDF instead of 3D print?
- Why servo instead of DC motor?
- Why bearing instead of a plain shaft hole?

**Response:**  
`[Write here]`

## 12.3 Items to Purchase Separately

| Item | Why Needed | Purchase Link | Latest Safe Date to Procure | Status |
|---|---|---|---|---|
| `[Item]` | `[Reason]` | `[Link]` | `[Date]` | `[Pending / Ordered / Received]` |
| `[Item]` | `[Reason]` | `[Link]` | `[Date]` | `[Pending / Ordered / Received]` |

## 12.4 Budget Summary

| Budget Item | Estimated Cost |
|---|---:|
| Electronics | `[Cost]` |
| Mechanical parts | `[Cost]` |
| Fabrication materials | `[Cost]` |
| Purchased extras | `[Cost]` |
| Contingency | `[Cost]` |
| **Total** | `[Cost]` |

## 12.5 Budget Reflection
If your cost is too high, what can be simplified, removed, substituted, or shared?

**Response:**  
`[Write here]`

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
`[Write here]`

## 13.2 Task Breakdown

| Task ID | Task | Owner | Estimated Hours | Deadline | Dependency | Status |
|---|---|---|---:|---|---|---|
| T1 | `[Finalize concept]` | `[Name]` | `2` | `[Date]` | `None` | `To Do` |
| T2 | `[Complete BOM]` | `[Name]` | `1` | `[Date]` | `T1` | `To Do` |
| T3 | `[Test electronics]` | `[Name]` | `2` | `[Date]` | `T1` | `To Do` |
| T4 | `[Build structure]` | `[Name]` | `4` | `[Date]` | `T1` | `To Do` |
| T5 | `[Write control code]` | `[Name]` | `4` | `[Date]` | `T3` | `To Do` |
| T6 | `[Integrate system]` | `[Name]` | `4` | `[Date]` | `T4, T5` | `To Do` |
| T7 | `[Playtest]` | `[Name]` | `2` | `[Date]` | `T6` | `To Do` |
| T8 | `[Refine and document]` | `[Name]` | `3` | `[Date]` | `T7` | `To Do` |

## 13.3 Responsibility Split

| Area | Main Owner | Support Owner |
|---|---|---|
| Concept and gameplay | `[Name]` | `[Name]` |
| Electronics | `[Name]` | `[Name]` |
| Coding | `[Name]` | `[Name]` |
| App | `[Name]` | `[Name]` |
| Mechanical build | `[Name]` | `[Name]` |
| Testing | `[Name]` | `[Name]` |
| Documentation | `[Name]` | `[Name]` |

---

# 14. Weekly Milestones

## 14.1 Four-Week Plan

### Week 1 — Plan and De-risk
Expected outcomes:
- [ ] Idea finalized
- [ ] Core interaction decided
- [ ] Sketches made
- [ ] BOM completed
- [ ] Purchase needs identified
- [ ] Key uncertainty identified
- [ ] Basic feasibility tested

### Week 2 — Build Subsystems
Expected outcomes:
- [ ] Electronics tests completed
- [ ] CAD / structure planning completed
- [ ] App UI started if needed
- [ ] Mechanical concept tested
- [ ] Main subsystems partially working

### Week 3 — Integrate
Expected outcomes:
- [ ] Physical body built
- [ ] Electronics integrated
- [ ] Code connected to hardware
- [ ] App connected if required
- [ ] First playable version exists

### Week 4 — Refine and Finish
Expected outcomes:
- [ ] Technical bugs reduced
- [ ] Playtesting completed
- [ ] Improvements made
- [ ] Documentation completed
- [ ] Final build ready

## 14.2 Weekly Update Log

| Week | Planned Goal | What Actually Happened | What Changed | Next Steps |
|---|---|---|---|---|
| Week 1 | `[Write here]` | `[Write here]` | `[Write here]` | `[Write here]` |
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
`[Write here]`

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



```

## 17.3 Version History

| Version | Date | What Changed | Why |
|---|---|---|---|
| `v1` | `[Date]` | `[Describe]` | `[Reason]` |
| `v2` | `[Date]` | `[Describe]` | `[Reason]` |
| `v3` | `[Date]` | `[Describe]` | `[Reason]` |

---

# 18. Final Outcome

## 18.1 Final Description
Describe the final version of your project.

**Response:**  
`[Write here]`

## 18.2 What Works Well
- `[Point 1]`
- `[Point 2]`
- `[Point 3]`

## 18.3 What Still Needs Improvement
- `[Point 1]`
- `[Point 2]`
- `[Point 3]`

## 18.4 What Changed From the Original Plan
How did the project change from the initial idea?

**Response:**  
`[Write here]`

---

# 19. Reflection

## 19.1 Team Reflection
What did your team do well?  
What slowed you down?  
How well did you manage time, tasks, and responsibilities?

**Response:**  
`[Write here]`

## 19.2 Technical Reflection
What did you learn about:
- electronics,
- coding,
- mechanisms,
- fabrication,
- integration?

**Response:**  
`[Write here]`

## 19.3 Design Reflection
What did you learn about:
- designing for play,
- delight,
- clarity,
- physical interaction,
- player understanding,
- iteration?

**Response:**  
`[Write here]`

## 19.4 If You Had One More Week
What would you improve next?

**Response:**  
`[Write here]`

---

# 20. Final Submission Checklist

Before submission, confirm that:
- [ ] Team details are complete
- [ ] Project description is complete
- [ ] Inspiration sources are included
- [ ] Player journey is written
- [ ] Sketches are added
- [ ] BOM is complete
- [ ] Purchase list is complete
- [ ] Budget summary is complete
- [ ] Mechanical planning is documented if applicable
- [ ] App planning is documented if applicable
- [ ] Code flowchart is added
- [ ] Task breakdown is complete
- [ ] Weekly logs are updated
- [ ] Risk register is complete
- [ ] Testing log is updated
- [ ] Playtesting notes are included
- [ ] Build photos are included
- [ ] Final reflection is written

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
- [ ] Approved to proceed
- [ ] Approved with changes
- [ ] Rework required before proceeding

**Instructor comments:**  
`[Instructor fills this section]`

## 22.2 Midpoint Review
`[Instructor fills this section]`

## 22.3 Final Review Notes
`[Instructor fills this section]`
