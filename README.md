# SKILL LAB PRATICAL HACKATHON

## Final Project README

> **Project Weight:** 100%  
> **Team Size:** 4/3 students  
> **Project Duration:** 16 hours  
> **Total Time Available:** 32 effort-hours per team  
> **Project Type:** Playful, interactive, technology-based experience

---

# Before you begin

## Fork and rename this repository

After forking this repository, rename it using the format:

`SKILLLAB_PROR-2026-TeamName`

### Example

`SKILLLAB_PROR-2026-AuroWizards`

Do not keep the default repository name.

---

# How to use this README

This file is your team’s **working project document**.

You must keep updating it throughout the build period.  
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

`Synapse`

## 1.2 Team Members

| Name                  | Primary Role                    | Secondary Role   | Strengths Brought to the Project |
| --------------        | ------------------------------- | --------------   | -------------------------------- |
| `Tanaya Balki`        | `[Electronics / Coding / App ]` | `Documentation`  | `Documentation,Raspberry Pi `|
| `Tushar Parmar`       | `[Electronics / Fabrication]`   | `[Coding]`       | `Material Handling, Hardware`    |
| `Om Rajbhar`          | `[Electronics / Fabrication]`   | `[Coding]`       | `Material Handling, Hardware`    |
| `Siddhai Thalkar`     | `[Electronics / Fabrication]`   | `[Coding]`       | `Documentation,Raspberry Pi`    |

## 1.3 Project Title

`"Smart Blind Stick"`

<img width="1600" height="1131" alt="image" src="https://github.com/user-attachments/assets/c64bfbd4-b3b7-43d9-83ad-c203a5aa11bc" />

## 1.4 One-Line Pitch

`An embedded assistive system designed to help visually impaired individuals navigate safely using smart sensor technology`

## 1.5 Expanded Project Idea

The Smart Blind Stick is an embedded systems project developed to assist visually impaired individuals in navigating their surroundings safely and independently. The system uses multiple sensors such as ultrasonic and IR sensors to detect nearby obstacles, pits, or stairs and alert the user through buzzer or vibration feedback.

The project combines embedded electronics, sensor integration, and wireless communication technologies to create a safer mobility solution. Additional features like emergency alert triggering and Bluetooth-based communication enhance the usability of the stick. The aim of the project is to provide an affordable, practical, and user-friendly assistive device using modern embedded system concepts.

---

# 2. Inspiration

## 2.1 References

List what inspired the project.

| Source Type | Title / Link                                                        | What Inspired You                                                                         |
| ----------- | ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `[Video]`   | `https://www.instagram.com/reel/DSVh31YE3gc/?igsh=Y2xtbG96aXF4dHYz` | `Understanding how technology can create interactive and practical real-world assistance systems` |
|    `[Research / Existing Concepts]`           | 	`An_Intelligent_and_Multi-Functional_Stick_for_Blind_People_Using_IoT` | `The idea of combining IoT technology, sensors, and embedded systems to improve safety and independence for visually impaired individuals inspired our project.` |
|             |                                                                     |                                                                                           |

## 2.2 Original Twist

What makes your project original?

The uniqueness of this project comes from its simple and practical design. Instead of connecting the stick directly to the internet, it uses Bluetooth to communicate with a smartphone, which reduces complexity and power usage. The project combines multiple features such as obstacle detection using both IR and ultrasonic sensors, a touch-based SOS system for emergencies, and location sharing through a mobile phone.

It also includes a temperature and humidity sensor, which can be useful for future improvements. Overall, the project stands out because it provides multiple safety features in a cost-effective and easy-to-use system.


---

# 3. Project Intent

## 3.1 User Journey 

A visually impaired person uses the smart blind stick while walking outside. As they move, the stick continuously checks for obstacles using its sensors. If something comes in the way, the system detects it and alerts the user through a buzzing sound, helping them avoid collisions.

The user does not need to do anything manually during normal use, as the system works automatically in the background. This makes walking safer and more comfortable.

If the user feels unsafe or needs help, they can press the touch sensor on the stick. This sends an emergency signal to their smartphone through Bluetooth. The phone then gets the user’s current location and sends it to family members or caregivers.

The stick acts as a reliable support system for daily use and emergencies. 

---

# 4. Definition of Success

## 4.1 Definition of “Usable”

The project is considered successful if it can detect obstacles correctly, send alerts to the smartphone without delay, and successfully deliver emergency messages. It should also be easy to use, lightweight, and reliable in real-world conditions.

## 4.2 Minimum Usable Version

What is the smallest version of this project that still delivers the core experience?

The minimum version of this project includes a Raspberry Pi, an ultrasonic sensor for obstacle detection, and a touch sensor for SOS. The system should be able to detect obstacles and send an emergency alert to a smartphone using Bluetooth. This basic setup is enough to provide the main safety feature.


## 4.3 Stretch Features

What features are nice to have but not essential?

1) Creating a custom mobile app instead of using messaging apps
2) Using a camera for object detection
3) Adding voice guidance for better navigation
4) Using a more accurate sensor instead of DHT11
5) Adding a GPS module directly to the stick
6) Detecting falls using motion sensors
7) Storing data for tracking and analysis

# 5. System Overview

## 5.1 Project Type

Check all that apply.

- [x] Electronics-based

- [ ] Mechanical

- [x] Sensor-based

- [ ] App-connected

- [ ] Motorized

- [x] Sound-based

- [ ] Light-based

- [x] Screen/UI-based

- [x] Fabricated structure

- [ ] Game logic based

- [x] Installation

- [ ] Other:

## 5.2 High-Level System Description


Input

The system receives input from:
Ultrasonic sensor for obstacle detection
IR sensor for detecting pits, holes, or stairs
Touch sensor for emergency activation
DHT11 sensor for environmental monitoring
Processing

All sensor data is processed by the Arduino microcontroller. The controller continuously analyzes distance and ground-condition data to determine possible danger situations.

Output

When obstacles or unsafe conditions are detected:
A buzzer or vibration motor alerts the user
Bluetooth module can send emergency notifications to a connected mobile device
Physical Structure

The sensors and electronics are mounted onto a walking stick structure in a compact and portable arrangement. The design is lightweight and easy to carry.

App Interaction

The Bluetooth module allows communication with a mobile application or smartphone for emergency alert features and future smart integrations.

## 5.3 Input / Output Map
   
| System Part              | Type          | What It Does                            |
|--------------------------|---------------|------------------------------------------|
| Ultrasonic Sensor        | Input         | Detects nearby obstacles                 |
| IR Sensor                | Input         | Detects pits, stairs, or ground changes  |
| Touch Sensor             | Input         | Triggers emergency alert                 |
| DHT11 Sensor             | Input         | Measures temperature/environment         |
| Raspberry Pi             | Processing    | Processes all sensor data                |
| Buzzer / Vibration Motor | Output        | Alerts the user about danger             |
| Bluetooth Module         | Communication | Sends alerts to connected device         |


---

# 6. System Design, Sketches and Visual Planning 

## 6.1 Concept Architecture/sketch/schematic

Add an early sketch of the full idea.

**Insert image below:**  
`[Upload image and link here]`

Example:

```md

```



## 6.2 Labeled Build Sketch/architecture/flow diagram/algorithm

Add a sketch with labels showing:

- structure,
- electronics placement,
- user touch points,
- moving parts,
- output elements.

**Insert image below:**  
`[Upload image and link here]`
<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/95637f31-b4e7-4427-a9e1-4b63fbeb0ac5" />

## 6.3 Approximate Dimensions

| Dimension        | Value   |
| ---------------- | ------- |
| Length           | `16 cm` |
| Width            | `16 cm` |
| Height           | `8 cm`  |
| Estimated weight | `400 g` |

---

# 7. Electronics Planning

## 7.1 Electronics Used

| Component                 | Quantity | Purpose                               |
| ------------------------- | --------:| ------------------------------------- |
| Raspberry Pi | `1` | Main processing and control unit |
| Ultrasonic Sensor (HC-SR04) | `1` | Detects nearby obstacles |
| IR Sensor | `1` | Detects pits, stairs, or holes | 
| DHT11 Sensor | `1` | Measures environmental temperature | 
| Touch Sensor | `1` | Triggers emergency alert | 
| Bluetooth Module (HC-05) | `1` | Sends alerts to connected device |
| Buzzer / Vibration Motor | `1` | Provides warning alerts to user | 
| Battery Pack | `1` | Powers the complete system | 
| Jumper Wires | `Multiple` | Electrical connections between components |

## 7.2 Wiring Plan

The Raspberry Pi acts as the central controller and is connected to all sensors and output devices through GPIO pins. The ultrasonic sensor is connected for obstacle detection using trigger and echo pins. The IR sensor is connected to detect pits, stairs, or sudden ground changes. The DHT11 sensor is connected to monitor environmental conditions, while the touch sensor is used to activate emergency alerts manually. The buzzer or vibration motor is connected to output pins to provide warning feedback to the user whenever danger is detected. The Bluetooth module is connected through UART communication pins to send emergency notifications or alerts to a connected mobile device. 

---

## 7.3 Circuit Diagram/architecture diagram

Insert a hand-drawn or software-made circuit diagram.

<img src="images/block diagram.jpg" width="867" height="1156" alt="" src="" />


# 7.4. Power Plan

| Question         | Response                                                                                                                                          |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Power Source |  |
| Voltage Required | `5V for Raspberry Pi and sensors` |
| Current Concerns | `Continuous sensor operation and Bluetooth communication may increase power consumption` |
| Safety Concerns | `Avoid short circuits, ensure proper insulation, and use regulated power supply connections` |
---

# 8. Software Planning/

## 8.1 Software Tools

| Tool / Platform                | Purpose                                        |
| ------------------------------ | ---------------------------------------------- |
| Python | Main programming language for Raspberry Pi | 
| Raspberry Pi OS | Operating system for Raspberry Pi | 
| GPIO Library | Sensor and output device interfacing |
| Bluetooth Communication | Sending alerts to connected mobile device |
| GitHub | Project documentation and version control |

## 8.2 Software Logic/Algorithm

- **Startup behavior:** The Raspberry Pi initializes GPIO pins, sensors, Bluetooth communication, and output devices such as the buzzer or vibration motor.
-  **Input handling:** The system continuously receives input from the ultrasonic sensor, IR sensor, touch sensor, and DHT11 sensor.
  -  **Sensor reading:** The ultrasonic sensor measures obstacle distance, the IR sensor detects pits or stairs, and the DHT11 sensor monitors environmental conditions.
  -   **Decision logic:** The Raspberry Pi analyzes sensor data to determine whether obstacles or unsafe conditions are present. If danger is detected within a threshold range, the system activates warning alerts.
  -    **Output behavior:** The buzzer or vibration motor alerts the user whenever an obstacle, pit, or unsafe condition is detected.
  -  **Communication logic:** The Bluetooth module sends emergency notifications or alert messages to a connected mobile device when the emergency touch sensor is activated.
  -   **Reset behavior:** The system continuously repeats sensor monitoring and automatically resets alerts once the danger condition is cleared.

    
## 8.3 Code Flowchart

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
<img width="1600" height="1200" alt="image" src="" />
<img width="1600" height="1200" alt="image" src="" />




# 9. Bill of Materials

## 9.1 Full BOM

| Item | Quantity | In Kit? | Need to Buy? | Estimated Cost (₹) | Material / Spec | Why This Choice? |
|------|----------|---------|--------------|--------------------|------------------|------------------|
| Raspberry Pi | 1 | Yes | No | 0 | Model with Bluetooth support | Main controller to process sensor data |
| Ultrasonic Sensor | 1 | Yes | No | 0 | 2–400 cm range | Detects obstacles at a distance |
| IR Sensor | 1 | Yes | No | 0 | Infrared proximity sensor | Detects very close obstacles |
| Touch Sensor | 1 | Yes | No | 0 | Capacitive touch module | Easy SOS trigger for user |
| DHT11 Sensor | 1 | Yes | No | 0 | Temp & humidity sensor | Environmental monitoring |
| Buzzer | 1 | No | No | 0 | 5V module | Alerts user when obstacle detected |
| Bluetooth Module  | 1 | Yes | No | 0 | HC-05 | For communication  |
| Battery Pack | 1 | No | Yes | 200 | Power bank / Li-ion | Portable power supply |
| Connecting Wires | Multiple | Yes | No | 0 | Jumper wires | Circuit connections |
| Stick Structure | 1 | No | No | 0 | PVC / metal rod | Physical support |

## 9.2 Material Justification

Explain why you selected your main materials and components.

**Response:**  
The Raspberry Pi is used because it can handle multiple sensors and supports Bluetooth communication.  
The ultrasonic sensor is used for long-range obstacle detection, while the IR sensor detects nearby objects. This combination improves accuracy.  
The touch sensor is easy to use and allows quick SOS triggering.  
The buzzer or vibration motor gives immediate feedback to the user.  
The DHT11 sensor is added for environmental monitoring and future improvements.  
A battery pack is used to make the system portable.


## 9.3 Items You chose

 Item | Why Needed | Purchase Source | Latest Safe Date | Status |
|------|------------|----------------|------------------|--------|
| Ultrasonic Sensor | Detect obstacles at a distance | Already available | Before testing | Received |
| DHT11 Sensor | Measure temperature and humidity | Already available | Before testing | Received |
| Buzzer / Vibration Motor | To alert user | Already available | Before testing | Received |
| Battery Pack | Power supply | Local store | Before final assembly | Received |
| Stick Structure | Mounting components | Already available | Before integration | Received |

## 9.4 Budget Summary

 Budget Item | Estimated Cost (₹) |
|-------------|--------------------|
| Electronics | 0 |
| Mechanical parts | 0 |
| Fabrication materials | 0 |
| Purchased extras | 0 |
| Contingency | 0 |
| **Total** | **0** |

## 9.5 Budget Reflection

If your cost is too high, what can be simplified, removed, substituted, or shared?

The project is low cost and affordable.  

---

# 10. Planning the Work

## 10.1 Team Working Agreement

Write how your team will work together.

Include:

- how tasks are divided,
- how decisions are made,
- how progress will be checked,
- what happens if a task is delayed,
- how documentation will be maintained.

**Response:**  


## 10.2 Task Breakdown

| Task ID | Task | Owner | Estimated Time | Deadline | Dependency | Status |
|--------|------|--------|-----------------|----------|------------|--------|
| T1 | Finalize concept | All | 15 mins| 30th April| None | Done |
| T2 | Collect components | All | 15 mins | 30th April | T1 | Done |
| T3 | Sensor interfacing | Om and Tushar | 2.5 hours | 30th April | T2 | Done |
| T4 | System integration | All| 1 hour | 30th April | T3 | Done |
| T5 | Testing & debugging | Om and Tushar | 30 mins | 1th May | T4 | Done |
| T6 | Documentation | Tanaya and Siddhai | 5 | 1th May | Ongoing | Ongoing |


## 10.3 Responsibility Split

| Area                 | Main Owner     | Support Owner |
| -------------------- | ----------     | ------------- |
| Concept              | `[Mrugendra]`  | `[Jyoti]`     |
| Electronics          | `[]`           | `[]`          |
| Coding               | `[]`           | `[]`          |
| Mechanical build     | `[]`           | `[]`          |
| Testing              | `[]`           | `[]`          |
| Documentation        | `[]`           | `[]`          |

---

# 11 hour Milestones

## 11.1 8-hour Plan(tentetively you may set)

### Bi Hour 1 — Plan and De-risk

Expected outcomes:

- [x] Idea finalized
- [x] Core interaction decided
- [x] Sketches made
- [x] BOM completed
- [x] Purchase needs identified
- [x] Key uncertainty identified
- [x] Basic feasibility tested

### Bi Hour 2 — Build Subsystems

Expected outcomes:

- [x] Electronics tests completed
- [x] CAD / structure planning completed
- [ ] App UI started if needed
- [x] Mechanical concept tested
- [x] Main subsystems partially working

### Bi Hour 3 — Integrate

Expected outcomes:

- [ ] Physical body built
- [x] Electronics integrated
- [x] Code connected to hardware
- [ ] App connected if required
- [x] First playable version exists

### Bi Hour 4 — Refine and Finish

Expected outcomes:

- [x] Technical bugs reduced
- [x] Playtesting completed
- [x] Improvements made
- [ ] Documentation completed
- [x] Final build ready

## 12.2  Update Log

| Days  | Planned Goal                          | What Actually Happened                                  | What Changed                                  | Next Steps                              |
|-------|---------------------------------------|----------------------------------------------------------|-----------------------------------------------|------------------------------------------|
| Day 1 | Finalize idea and components          | Idea finalized, sensors identified                       |Added temperature sensor        | Start sensor testing                     |
| Day 1 | Sensor interfacing                    | Ultrasonic, IR, touch sensors tested                     | Added buzzer for feedback                      | Begin Bluetooth setup                    |
| Day 1 | Integration                          | Sensors + buzzer + Bluetooth working together            | Focus shifted to SOS-only messaging            | Test full system                         |
| Day 1 | Testing             | System tested, documentation started          | Simplified messaging     | Continued with documentation           |



---

# 13. Risks and Unknowns

## 13.1 Risk Register

| Risk                                                | Type        | Likelihood | Impact | Mitigation Plan                                                                 | Owner   |
|-----------------------------------------------------|------------|------------|--------|----------------------------------------------------------------------------------|---------|     
| Power supply issues                                | Hardware   | Medium     | High   | Use stable battery, check voltage regularly                                     | Tushar  |
| Delay in SOS message delivery                      | System     | Low        | High   | Optimize Bluetooth communication and message trigger                            | Tushar |
| Loose connections or hardware failure              | Hardware   | Medium     | Medium | Proper wiring, secure mounting                                                  | Om      |         


## 13.2 Biggest Unknown Right Now

What is the single biggest uncertainty in your project at this stage?

The biggest uncertainty in the project is the reliability of Bluetooth communication in real-world conditions. Factors like signal range, interference, and device compatibility can affect how quickly and consistently the SOS message is transmitted. Further testing is required to ensure stable performance. 


---

# 14. Testing 

## 14.1 Technical Testing Plan

| What Needs Testing     | How You Will Test It                                                                 | Success Condition                                                                                    |
| ---------------------- | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------- |
| `[Wifi connection]`    | `[Check if motor spins via app button]`                                              | `[Both motors accurately respond to wifi signals]`                                                   |
## 14.2 Testing and Debugging Log

| Date         | Problem Found                              | Type        | What You Tried                                      | Result        | Next Action                                  |
|--------------|--------------------------------------------|------------|-----------------------------------------------------|--------------|----------------------------------------------|
| 30 April   | SOS not triggering consistently            | Hardware   | Checked touch sensor connections                    | Fixed        | Secure connections properly                  |


## 14.3 Playtesting Notes

| Tester      | What They Did                        | What Confused Them                    | What They Enjoyed                         | What You Will Change                          |
| ----------- | ------------------------------------ | ------------------------------------- | ----------------------------------------- | --------------------------------------------- |
| `Gopal` | `Tried navigating through obstacles` | `Some obstacles ewren't clear enough` | `Liked projection + real car interaction` | `Add a slight red highlight around obstacles` |


---

# 15. Build Documentation

## 15.1 Fabrication Process(if any)

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
The fabrication process involved assembling the physical structure of the smart blind stick and integrating all electronic components properly.

**Design and Planning:**  
The layout of sensors and components was first planned to ensure proper placement on the stick. The positions were chosen so that obstacle detection is accurate and the touch sensor is easily accessible.

**Assembly:**  
All components such as the Raspberry Pi, sensors, and battery pack were mounted onto the stick using basic supports and fastening methods. Care was taken to keep the system compact and lightweight.

**Wiring:**  
Connections between sensors and the Raspberry Pi were made using jumper wires. Proper routing was done to avoid loose connections and ensure stability during use.

**Mounting:**  
Sensors like the ultrasonic and IR sensor were fixed at suitable angles to detect obstacles effectively. The touch sensor was placed where the user can easily access it.

**Power Setup:**  
A portable battery pack was connected to power the system, making it suitable for real-world use.

**Finishing:**  
The structure was checked for stability and comfort. Loose wires were secured, and the system was adjusted to ensure ease of handling.

## 16 Build Photos

Add photos throughout the project.

Suggested images:

- early sketch,
- prototype,
- electronics testing,
- mechanism test,
- app screenshot,
- final build.
- <img width="960" height="1280" alt="WhatsApp Image 2026-04-24 at 9 46 02 AM (1)" src="https://github.com/user-attachments/assets/74baa570-5770-483e-be6d-d2f03386e37c" />





# 17. Final Outcome

## 17.1 Final Description

Describe the final version of your project.

**Response:**  


## 17.2 What Works Well



## 17.3 What Still Needs Improvement


## 17.4 What Changed From the Original Plan

How did the project change from the initial idea?

**Response:**  


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
<img width="1131" height="1600" alt="image" src="" />

---


---


