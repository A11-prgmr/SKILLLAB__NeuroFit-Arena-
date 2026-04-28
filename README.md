
---

# 1. Team Identity

## 1.1 Studio / Group Name

`NeuroFit Arena`

## 1.2 Team Members

| Name           | Primary Role                    | Secondary Role | Strengths Brought to the Project |
| -------------- | ------------------------------- | -------------- | -------------------------------- |
| `Anshul Tatke ` | `[Electronics / Coding ]` | `Documentation`  | `Documentation, Hardware`|
| `Rudra Valecha`  | `[Electronics / Hardware]`   | `[Coding]`     | `Material Handling, Hardware`    |
| `Varad Sawant`  | `[Hardware]`   | `[Design]`     | `Material Handling, Hardware`    |
| `Neeraj Topale`  | `[ Design]`   | `[Structuring]`     | `Design`    |
<img width="1600" height="1131" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/Group9.jpeg" />
## 1.3 Project Title

`"NeuroFit Arena"`



<img width="1600" height="1131" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/Title.png" />

## 1.4 One-Line Pitch

`NeuroFit Arena is an adaptive multi-sensor system that gamifies cognitive and physical training through real-time interactive challenges.
`

## 1.5 Expanded Project Idea

##  NeuroFit Arena: Adaptive Cognitive & Physical Training System

NeuroFit Arena is an interactive multi-mode training platform that combines cognitive challenges, physical activity, and biometric sensing into a single intelligent system. Designed using the Shrike Vicharak Pico (RP2040), the project transforms simple sensors into an engaging environment that enhances human performance through real-time feedback and adaptive difficulty.

The system features four distinct modes—Reaction, Memory, Motion, and Grip Strength—each targeting a different aspect of human ability. Reaction mode measures reflex speed, Memory mode improves pattern recognition, Motion mode encourages physical coordination using distance sensing, and Grip mode evaluates strength and control using a force-sensitive resistor.

What sets NeuroFit Arena apart is its ability to dynamically adjust difficulty based on user performance, creating a personalized training experience. By integrating multiple sensing techniques and combining them with interactive gameplay, the system goes beyond traditional electronics projects and moves toward a holistic human–machine interaction model.

This project demonstrates how embedded systems can be applied in areas such as fitness training, cognitive development, and rehabilitation, making it both innovative and practically relevant.

---

# 2. Philosophy Fit

## 2.1 Experience, Not Social Problem

This project focuses on creating an interactive and engaging user experience rather than solving a specific social problem. The goal is to combine mental and physical activities into a single system that users can enjoy while improving their cognitive and reflex abilities.

In today’s digital world, most games are limited to screens. This project brings interaction into the physical world, where users must move, react, remember, and apply strength in real-time. It transforms traditional gaming into an immersive experience involving both the body and the brain.




# 3. Inspiration
This game intends to improve one's reaction time, memory along with keeping the person physically active.
Our inspiration to create this game was mainly about wellbeing. The game aims to help kids improve their memory and reaction time while entertaining them, whereas it also targets aging adults to help them regularly sharpen their hand-eye co-ordination and brush their memory.
Overall we aim to make it an all-ages game inclusive to everyone

## 3.1 References

List what inspired the project.

| Source Type | Title / Link                                                        | What Inspired You                                                                         |
| ----------- | ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `[Video]`   | `https://youtu.be/ah5ioznsX3k?si=t2rXrwfmkssxhTrY` | `Memory based game, we implemented some parts of it into our project` |
|     '[AI Tools]'      |                                                                   |    Used to help enhance our project                                                                                       |
|             |                                                                     |                                                                                           |

## 3.2 Original Twist

What makes your project original?

**Response:**  
What makes this project unique is the integration of multiple skill-based games into one single system. Instead of focusing on just one aspect like memory or reaction, this project combines:

Reflex testing (Reaction Mode)
Cognitive ability (Memory Mode)
Physical activity (Motion Mode)
Strength measurement (GripX Mode)

The originality lies in:

Multi-mode design in a single device
Use of real-world sensors for gameplay
Adaptive difficulty system based on player performance
Combination of electronics, mechanics, and human interaction

---
 
# 4. Project Intent

## 4.1 User Journey 
The user will choose one of the four modes available in the game.
According to the user's choice, the respective game will be selected.
For Game one and two, it is simple hand-eye co-ordination game where in game one the user has to touch the button according to the led.
In game two, the player will need to touch the buttons in order the leds blink.
For Game 4 one simply needs to grip the stress ball and press it.


---

## 5. Definition of Success

### 5.1 Definition of “Usable”

The system is considered usable if it can reliably detect user inputs through touch sensors, respond with correct LED outputs, and accurately measure and display reaction time. The interface should be intuitive, with clear visual feedback, allowing users to play without prior instructions.

---

### 5.2 Minimum Usable Version

The minimum usable version of the project consists of:

* 3 LEDs and 3 touch sensors
* Random LED activation
* Correct input detection
* Reaction time calculation using timer functions
* Output displayed via serial monitor

This version delivers the core experience of a reaction-based game and demonstrates real-time interaction between user and system.

---

### 5.3 Stretch Features

The following features enhance the system but are not essential:

* Multiple game modes (Memory, Motion, Grip strength)
* LCD display for real-time score and feedback
* Buzzer for audio interaction
* Adaptive difficulty based on user performance
* Multi-player or scoring system
* Biometric input using FSR (grip strength analysis)

These features improve engagement and functionality but are not required for the basic operation of the system.


---

# 6. System Overview

## 6.1 Project Type

Check all that apply.

- [x] Electronics-based

- [ ] Mechanical

- [x] Sensor-based

- [ ] App-connected

- [x] Motorized

- [x] Sound-based

- [x] Light-based

- [x] Screen/UI-based

- [ ] Fabricated structure

- [x] Game logic based

- [ ] Installation

- [ ] Other:

## 6.2 High-Level System Description

Explain how the system works in simple terms.
                                                     |

## 6.2 High-Level System Description

**Response:**
NeuroFit Arena is an interactive system that uses sensors and simple electronics to create engaging training games. The system takes input from the user through touch sensors, motion sensing, and grip pressure, and processes this information using the Pico microcontroller.

Based on the input, the system responds by lighting LEDs, generating sounds, and calculating performance metrics such as reaction time. Each game mode focuses on a different skill, such as reflexes, memory, movement, or strength. The system continuously reads inputs, processes them, and gives instant feedback, making the interaction real-time and engaging.

---

## 6.3 Input / Output Map

| System Part          | Type    | What It Does                                     |
| -------------------- | ------- | ------------------------------------------------ |
| Touch Sensors        | Input   | Detect user touch to register responses in games |
| Ultrasonic Sensor    | Input   | Measures distance to detect body movement        |
| Force Sensor (FSR)   | Input   | Measures grip pressure for strength-based mode   |
| Pico Microcontroller | Process | Processes all inputs and controls outputs        |
| LEDs                 | Output  | Provide visual signals for gameplay              |
| Buzzer               | Output  | Gives audio feedback during interaction          |
| Serial Monitor / LCD | Output  | Displays results like reaction time and scores   |

---

# 7. Sketches and Visual Planning

## 7.1 Concept Sketch

Add an early sketch of the full idea.

**Insert image below:**  
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/image.png" />

## 7.2 Labeled Build Sketch

Add a sketch with labels showing:

- structure,
- electronics placement,
- user touch points,
- moving parts,
- output elements.

**Insert image below:**  
`[Upload image and link here]`
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/Concept.jpeg" />

## 7.3 Approximate Dimensions

| Dimension        | Value   |
| ---------------- | ------- |
| Length           | `16 cm` |
| Width            | `16 cm` |
| Height           | `8 cm`  |
| Estimated weight | `400 g` |

---

# 8. Electronics Planning

## 8.1 Electronics Used

| Component                 | Quantity | Purpose                               |
| ------------------------- | --------:| ------------------------------------- |
| `[Shrike Pi Pico]`                 | `1`      | `[Main controller]`                   |
| `[Ultrasonic ]`    | `2`      | `[]`                    |
| `[FSR]`             | `2`      | `[Grip strength]`                     |
| `LEDs` | `3`      | `[For reaction and memory game ]` |
| `[Touch Sensor]`        | `3`      | `[As buttons]`                       |
| `[Buzzer]`        | `1`      | `[Indication]`                       |
| `[Resistors ]`        | `As requirement`      | `[Regulation]`                       |
|`[I/O board ]`        | `1`      | `[Used to switch between modes]`                       |

## 8.2 Wiring Plan

Describe the main electrical connections.
 Overview

The system consists of three LEDs for visual output and three touch sensors for user input. All components are connected to the Shrike Vicharak Pico Board using GPIO pins, with common power and ground rails on a breadboard.

 Power Distribution
3.3V from Pico → Breadboard positive rail
GND from Pico → Breadboard ground rail
All components share common VCC and GND

LED Connections (Outputs)

Each LED is connected to a GPIO pin through a current-limiting resistor.

LED	GPIO Pin	Connection
LED 1	GP5	GP5 → 1kΩ resistor → LED → GND
LED 2	GP6	GP6 → 1kΩ resistor → LED → GND
LED 3	GP7	GP7 → 1kΩ resistor → LED → GND

 Touch Sensor Connections (Inputs)

Each touch sensor module is connected as follows:

Sensor	GPIO Pin	Connection
Touch 1	GP21	OUT → GP21, VCC → 3.3V, GND → GND
Touch 2	GP22	OUT → GP22, VCC → 3.3V, GND → GND
Touch 3	GP23	OUT → GP23, VCC → 3.3V, GND → GND

 Signal Flow
Touch sensor detects user input → sends HIGH signal to GPIO
Pico processes input → activates corresponding LED
Reaction time is calculated and displayed via serial output

**Response:**  


## 8.3 Circuit Diagram

Insert a hand-drawn or software-made circuit diagram.

**Insert image below:**  
`[Upload image and link here]`
<img width="867" height="1156" alt="" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/Circdiag1n2.jpeg" />
<img width="867" height="1156" alt="" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/circuitfinal.jpeg" />

# 9. Power Plan

| Question         | Response                                                                                                                                          |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Power source     | `Through USB`                                                                                                                           |
| Voltage required | `5V via USB input, internally regulated to 3.3V for GPIO and sensors`                                                                  |
| Current concerns | `System is low-power (LEDs, touch sensors, buzzer). Total current draw is minimal (<500 mA), well within USB limits. Avoid powering high-current devices like motors directly from the board`                                       |
| Safety concerns  | `Ensure proper wiring, avoid short circuits on breadboard, use current-limiting resistors for LEDs, and do not exceed 3.3V on GPIO pins` |

---

# 10. Software Planning

## 10.1 Software Tools

| Tool / Platform                | Purpose                                        |
| ------------------------------ | ---------------------------------------------- |
| `[MicroPython]`                | `Control Shrike`                                |

## 10.2 Software Logic

Describe what the code must do.

The software controls the overall functioning of the NeuroFit Arena by managing inputs, processing logic, and generating outputs in real time.

###  Startup Behavior

On power-up, the system initializes all GPIO pins, serial communication, and connected peripherals (LEDs, touch sensors, buzzer). A startup message is displayed, and the system enters standby mode awaiting game initiation.

---

###  Input Handling

User inputs are received through touch sensors/buttons. Each input is continuously monitored using digital reads. Debouncing or slight delays are used to prevent false triggering.

---

### Sensor Reading

The system reads data from sensors such as touch inputs and, in extended modes, ultrasonic or force sensors. Values are sampled periodically and processed to ensure stable readings.

---

### Decision Logic

The core logic determines:

* Random selection of LED (stimulus generation)
* Matching of correct input with active LED

* Validation of correct vs incorrect responses

---

### 💡 Output Behavior

Based on the logic:

* LEDs indicate the active stimulus
* Serial monitor displays reaction time results
* Optional buzzer provides audio feedback
* LCD (if used) shows game status and scores

---

### 🔗 Communication Logic

The system communicates results via serial output for debugging and performance tracking. This can be extended to Bluetooth or other modules if required.

---

### 🔁 Reset Behavior

After each round:

* Outputs are reset (LED OFF)
* Variables are cleared or reinitialized
* System waits for the next cycle with a random delay, ensuring unpredictable gameplay

---

Overall, the software follows a loop-based execution model where inputs are continuously monitored, processed, and responded to in real time.



## 10.3 Code Flowchart
Insert a flowchart showing your code logic.


**Insert image below:**  
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/Block%20diagram.jpeg" />





# 11. Bill of Materials

## 11.1 Full BOM

| Item                             | Quantity | In Kit? | Need to Buy? | Estimated Cost | Material / Spec               | Why This Choice?          |
| -------------------------------- | --------:| ------- | ------------ | --------------:| ----------------------------- | ------------------------- |
| `[Vicharak Shrike Lite]`                        | `1`      | `Yes`   | `No`         | `0`            | `38 Pin Shrike`                | `[To control components]` |
| `[Touch sensors]`                 | `[3]`    | `[Yes]` | `[No]`       | `0`            | `[]`                     | `[To drive both motors]`  |
| `[LEDs]`          | `[3]`    | `[No]`  | `[Yes]`      | `[150]`        | `[]` | `[]`    |
| `[Force Sensitive Resistor]`               | `[1]`    | `[No]`  | `[Yes]`      | `[75]`         |                               |                           |
| `[I/O shield]`                        | `1`      | `Yes`   | `No`         | `0`            | ``                | `[As UI]` |
| `[Stress buster sponge ball]`                        | `1`      | `Yes`   | `No`         | `0`            | ``                | `[Use along FSR]` |
| `[Breadboard and connecting wires]`                        | `1`      | `Yes`   | `No`         | `0`            | `for connections`                | `[Connections]` |
## 11.2 Material Justification

The components used in this project were selected to achieve a balance between functionality, simplicity, and real-time interaction. The Shrike Vicharak Pico Board (RP2040) was chosen as the main controller due to its reliable performance, it was also instructed to use RP2040 by our mentor, sufficient GPIO availability, and support for fast input/output operations required for real-time games.

LEDs were used as visual indicators because they provide clear and immediate feedback to the user during gameplay, especially in reaction-based modes. Touch sensors were selected instead of mechanical buttons to ensure smoother and faster input detection with minimal physical effort, improving user experience.

The ultrasonic sensor was included for motion detection due to its accuracy in measuring distance changes, making it suitable for physical activity-based challenges. A Force Sensitive Resistor (FSR) was used for grip strength measurement, enabling the system to capture analog input and extend the project into biometric sensing.

A buzzer was added to provide audio feedback, enhancing interactivity and user engagement. All components were chosen to be low-power and compatible with 3.3V operation, allowing the entire system to be powered safely through USB without requiring additional power circuits.


## 11.3 Items You chose

| Item                 | Why Needed               | Purchase Link | Latest Safe Date to Procure | Status       |
| -------------------- | ------------------------ | ------------- | --------------------------- | ------------ |
| `Shrike Vicharak Pico Board` | `Main controller for processing and I/O operations`   | `Provided / Lab`     | `Already available`                | `[Available]` |
| `LEDs (3x)`     | `` | `Visual stimulus for reaction and game feedback` | `Lab`            | `Available` |
| `Touch Sensors`   | `User input for interaction and response detection`         | `Lab` | `already availabe`            | `Recieved`   |
| `Force Sensitive Resistor (FSR)`   | `Grip strength measurement (biometric input)`         | `Lab` | `already availabe`            | `Recieved`   |
| `Buzzer`   | `Audio feedback for alerts and interaction`         | `Lab` | `already availabe`            | `Recieved`   |
| `Breadboard & Wires`   | `Circuit prototyping and connections`         | `Lab` | `already availabe`            | `Recieved`   |


## 11.4 Budget Summary

| Budget Item                               | Estimated Cost (INR)      |
| ----------------------------------------- | ------------------------- |
| Electronics (Pico, sensors, LEDs, buzzer) | [400]                     |
| Mechanical parts                          | [0]                       |
| Fabrication materials                     | [0 (Available on campus)] |
| Purchased extras                          | [0]                       |
| Contingency                               | [100]                     |
| **Total**                                 | **[500]**                 |

---

## 11.5 Budget Reflection

The overall cost of the project is low because most components were available in the lab, and the system does not require expensive hardware such as motors, drivers, or external power modules. If cost reduction was necessary, components like the ultrasonic sensor or buzzer could be optionally removed without affecting the core functionality of the reaction-based system.

Additionally, LEDs and touch sensors can be shared across multiple modes, reducing the need for duplicate hardware. The use of USB power eliminates the need for batteries or power management circuits, further minimizing cost. Overall, the design is cost-efficient, scalable, and suitable for educational and prototype applications.

---

# 12. Planning the Work

## 12.1 Team Working Agreement
After the team discussed the Ideation, the team divided the work and assigned the tasks
Anshul worked on the complete documentation.
Rudra and Varad worked on prototyping and checking the working of sensors
Niraj worked on the design and structuring of our game.
Overall, every member contributed to every section wherever help was required.
**Response:**  


## 12.2 Task Breakdown

| Task ID | Task                    | Owner    | Estimated Hours | Deadline     | Dependency | Status |
| ------- | ----------------------- | -------- | ---------------:| ------------ | ---------- | ------ |
| T1      | `[Finalize concept]`    | `[Both]` | `2`             | `1st April`  | `None`     | `Done` |


## 12.3 Responsibility Split

| Area                 | Main Owner | Support Owner |
| -------------------- | ---------- | ------------- |
| Concept              | `[Anshul]`  | `[Rudra]`    |
| Electronics          | `[Rudra]`       | `[Varad]`     |
| Coding               | `[Rudra]`       | `[Anshul]`     |
| Mechanical build     | `[Varad]`       | `[Neeraj]`    |
| Testing              | `[Rudra]`       | `[Varad,Anshul]`    |
| Documentation        | `[Anshul]`       | `[]`     |

---

# 13. 2 hour Milestones

## 13.1 8-hour Plan

### Bi Hour 1 — Plan and De-risk

Expected outcomes:

- [x] Idea finalized
- [x] Core interaction decided
- [x] Sketches made
- [x] BOM completed
- [x] Purchase needs identified
- [ ] Key uncertainty identified
- [x] Basic feasibility tested
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/Update1.jpeg" />

### Bi Hour 2 — Build Subsystems

Expected outcomes:

- [x] Electronics tests completed
- [ ] structure planning completed
- [x] Mechanical concept tested
- [x] Main subsystems partially working
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/Update2jpeg.jpeg" />

### Bi Hour 3 — Integrate

Expected outcomes:

- [x] Physical body built
- [x] Electronics integrated
- [x] Code connected to hardware
- [x] First playable version exists
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/up3.jpeg" />

### Bi Hour 4 — Refine and Finish

Expected outcomes:

- [x] Technical bugs reduced
- [x] Playtesting completed
- [x] Improvements made
- [x] Documentation completed
- [x] Final build ready
 <img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/Final.jpeg" />

## 13.2  Update Log

| Week   | Planned Goal   | What Actually Happened | What Changed   | Next Steps     |
| ------ | -------------- | ---------------------- | -------------- | -------------- |
| Hour 1 | `[Checking Game 1 working ]` | `[Prototype obtained]`         | `[Shifted to Thonny ]` | `[Trying Arduino IDE]` |
| Hour 2 | `Checking Game 2 working  ]` | `[Prototype obtained,LED stopped working]`         | `[]` | `[Change of LEDs]` |
| Hour 3 | `[Game 3 Completion]` | `[Game 3 code gave multiple errors]`         | `[]` | `[Rechecking]` |
| Hour 4 | `[Redo Game 3]` | `[]`         | `[Still not functional]` | `[Move on to Game 4]` |
| Hour 5 | `[Start on game 4]` | `[Game 4 functionality checked]`         | `[]` | `[Start working on final check]` |
| Hour 6 | `[Designing and structuring]` | `[work on box continued]`         | `[Final design obtained]` | `[Start pitch and presentation]` |
| Hour 7 | `[]` | `[]`         | `[]` | `[]` |

---


## 14. Risks and Unknowns

### 14.1 Risk Register

| Risk                                         | Type      | Likelihood | Impact | Mitigation Plan                                                   | Owner         |
| -------------------------------------------- | --------- | ---------- | ------ | ----------------------------------------------------------------- | ------------- |
| Unstable touch sensor readings               | Technical | Medium     | Medium | Add small delays (debouncing), ensure proper wiring and grounding | [Team Member] |
| Incorrect reaction time measurement          | Technical | Low        | High   | Use `millis()` correctly, test timing logic multiple times        | [Team Member] |
| Loose wiring on breadboard                   | Technical | Medium     | High   | Double-check connections, keep wiring neat and secure             | [Team Member] |
| Power fluctuations from USB                  | Technical | Low        | Medium | Use reliable USB source and cable, avoid overloading the board    | [Team Member] |
| Sensor calibration issues (FSR / ultrasonic) | Technical | Medium     | Medium | Test and adjust threshold values before final demo                | [Team Member] |
| Integration bugs between modes               | Technical | Medium     | High   | Test each mode separately, then integrate step-by-step            | [Team Member] |

---

### 14.2 Biggest Unknown Right Now

The biggest uncertainty in our project is ensuring consistent and accurate sensor readings across all modes, especially when integrating multiple inputs like touch, motion, and grip sensing. Since different sensors behave differently in real-world conditions, maintaining stable performance during the final demo is a key challenge.


---

# 15. Testing 

## 15.1 Technical Testing Plan

| What Needs Testing     | How You Will Test It                                                                 | Success Condition                                                                                    |
| ---------------------- | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------- |
| `[Wifi connection]`    | `[Check if motor spins via app button]`                                              | `[Both motors accurately respond to wifi signals]`                                                   |
                       |
## 15.2 Testing and Debugging Log

| Date          | Problem Found                         | Type         | What You Tried                                | Result               | Next Action                                    |
| ------------- | ------------------------------------- | ------------ | --------------------------------------------- | -------------------- | ---------------------------------------------- |
| `18th April`  | `Car not balancing properly`          | `Mechanical` | `Add low-friction caster support to one side` | `Worked`             | `improve caster structure`                     |


## 15.3 Playtesting Notes

| Tester      | What They Did                        | What Confused Them                    | What They Enjoyed                         | What You Will Change                          |
| ----------- | ------------------------------------ | ------------------------------------- | ----------------------------------------- | --------------------------------------------- |
| `Gopal` | `Tried navigating through obstacles` | `Some obstacles ewren't clear enough` | `Liked projection + real car interaction` | `Add a slight red highlight around obstacles` |


---

# 16. Build Documentation

## 16.1 Fabrication Process

Describe how the project was physically made.

 Physical Implementation

The project was physically built using a breadboard-based prototyping approach centered around the Shrike Vicharak Pico Board. The Pico was powered via USB and placed on the breadboard, with its 3.3V and GND pins distributed across the power rails to supply all components.

Three LEDs were connected to GPIO pins through current-limiting resistors and placed visibly on the breadboard to act as visual indicators. Three touch sensors were mounted and connected to GPIO input pins, with their VCC and GND connected to the common power rails. Care was taken to keep wiring short and organized to ensure stable signal transmission.

Additional components such as the buzzer and sensors (ultrasonic and FSR for extended modes) were connected in a modular manner, allowing easy integration and testing without redesigning the base circuit. All connections were made using jumper wires, and the setup was tested incrementally—starting with basic LED control, followed by input detection, and finally integrating full game logic.

The overall design prioritized simplicity, and ease of debugging, making it suitable for rapid prototyping and demonstration within the hackathon timeframe.



## 16.2 Build Photos

All the build photos are attached below

<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/working.jpeg" />
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/working2.jpeg" />
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/working3.jpeg" />
<img width="1600" height="1200" alt="image" src="https://github.com/A11-prgmr/SKILLLAB__NeuroFit-Arena-/blob/main/images/working4.jpeg" />






## 17. Final Outcome

### 17.1 Final Description

The final version of NeuroFit Arena is a multi-mode interactive system built using the Shrike Vicharak Pico Board. It combines cognitive and physical training through different game modes, including reaction-based input using LEDs and touch sensors, motion detection using sensors, and grip strength measurement using an FSR.

The system provides real-time feedback through LEDs, serial output, and optional audio signals. It is designed to be modular, allowing additional modes and features to be integrated easily. The final implementation successfully demonstrates real-time interaction, sensor integration, and adaptive gameplay logic.

---

### 17.2 What Works Well

* Accurate reaction time measurement using timer functions
* Reliable touch sensor input with minimal delay
* Clear visual feedback through LEDs
* Smooth integration of multiple components
* Low power operation using USB without stability issues
* Modular design allowing easy expansion

---

### 17.3 What Still Needs Improvement

* Addition of LCD display for better user interface
* Improved sensor calibration for motion and grip modes
* Enhanced noise filtering for more stable readings
* More advanced scoring and data tracking system
* Better physical casing for durability and presentation
* The mode 3 game which focused on physical movement was not done sucessfully and need work on it
---

### 17.4 What Changed From the Original Plan

Initially, the project idea involved more complex hardware components such as motors and additional control systems. However, the design was simplified to focus on sensor-based interaction and real-time gameplay using the Shrike Pico Board.

The shift allowed for faster implementation, improved reliability, and better focus on user interaction rather than mechanical complexity. Additional features like multi-mode gameplay and biometric sensing (grip strength) were introduced, making the final system more innovative and user-centric compared to the original plan.

We also planned for 4 game modes, out of which we were able to sucesfully implement 3 modes.

---

# 18. Reflection

## 18.1 Team Reflection

What did your team do well?  
What slowed you down?  
How well did you manage time, tasks, and responsibilities?

**Response:**  


## 18.2 Technical Reflection

What did you learn about:

- electronics,
- coding,
- mechanisms,
- fabrication,
- integration?

**Response:**  


## 18.3 Design Reflection

What did you learn about:

- designing ,
- delight,
- clarity,
- physical interaction,
- understanding,
- iteration?

**Response:**  


## 18.4 If You Had One More hour

What would you improve next?

**Response:**  

` `

---
# 18. Reflection

## 18.1 Team Reflection

**Response:**
As a team, we performed rather well, as we divided responsibilities effectively, some working on wiring and hardware assembly while others were busy coding. The process of communication proved to be rather efficient, as we were exchanging information frequently while doing tests and debugging the code and device.

Initially, however, the problem was the lack of clarity concerning the actual plan of actions, since we took longer than expected discussing the project concept. Yet when we finally agreed upon something and settled the issue of what should be accomplished by now, we managed our schedule well.

---

## 18.2 Technical Reflection

**Response:**
The practical aspect of this project allowed us to learn how sensors and microcontrollers interact within an interactive system in practice. We have become fully aware of the significance of proper connections in order for the whole system to function properly.

As far as programming was concerned, it is safe to say that the project gave us a lot of opportunities to practice logical thinking.

Another important lesson from the assignment was the complexity involved in integrating the components as everything needed to be well synchronized which turned out to be difficult but also very rewarding.

---

## 18.3 Design Reflection

**Response:**
It turns out that a project should not only be functional, but it should also be enjoyable to operate. The simplicity of user interactions, such as the LEDs and touch sensor input, makes the project much easier for others to use.

The importance of gradual improvements through testing has also become apparent for us; slight modifications in the placement and logic have led to significant changes in system behavior. The main priorities were clear logic and interactivity.

## 18.4 If You Had One More Hour

**Response:**
In case there was one more hour available to work on our project, the most immediate improvement would be related to visualization of the output, possibly through an LCD display. In addition to this, we would improve sensor readings by making them consistent.

Another area where improvement could be applied is physical construction, for example, optimizing wiring.

Also,
If we had more time we would work on the mode we could not finish properly and ultimately had to scrap it due to time constraints

# 19. Final Submission Checklist

Before submission, confirm that:

- [x] Team details are complete
- [x] Project description is complete
- [x] Inspiration sources are included
- [x] Sketches are added
- [x] BOM is complete
- [x] Purchase list is complete
- [x] Budget summary is complete
- [x] Mechanical planning is documented if applicable
- [ ] App planning is documented if applicable
- [x] Code flowchart is added
- [x] Task breakdown is complete
- [x] Weekly logs are updated
- [x] Risk register is complete
- [x] Testing log is updated
- [x] Playtesting notes are included
- [x] Build photos are included
- [x] Final reflection is written

---


---


