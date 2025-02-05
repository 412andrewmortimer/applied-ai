# 2.1 Agents and Environments

## Overview
An **agent** is an entity that perceives its environment through **sensors** and acts upon the environment through **actuators**. The interaction between agents and environments is central to the study of artificial intelligence.

---

## **Key Concepts**

### **Agent**
- An agent is defined by:
  - **Sensors**: Devices or components that perceive the environment.
  - **Actuators**: Devices or components that affect the environment through actions.

- **Agent Function**: A mapping from percept sequences to actions:

- **Agent Program**: The implementation of the agent function that runs on a physical device (architecture).

---

### **Environment**
- The **environment** is the external world that the agent interacts with.
- The environment provides **percepts** to the agent via sensors and receives **actions** via actuators.

---

### **Agent-Environment Interaction**
- Interaction can be visualized as:
!!!example
    ```mermaid
    sequenceDiagram
    participant Environment
    participant Sensors
    participant Agent
    participant Actuators

    Environment->>Sensors: Generate percepts
    Sensors->>Agent: Pass percepts to Agent Program
    Agent->>Agent: Process percept sequence
    Agent->>Actuators: Select action
    Actuators->>Environment: Execute action
    ```
    !!!info
        **Agent → Sensors → Percepts → Environment → Actions → Actuators → Agent**

---

## **Examples of Agents**
| **Agent**              | **Sensors**            | **Actuators**       | **Environment**           |
|-------------------------|------------------------|---------------------|---------------------------|
| Self-Driving Car        | Cameras, GPS, LIDAR   | Steering, Brakes    | Roads, Traffic            |
| Medical Diagnosis System| Keyboards, Scanners   | Recommendations     | Medical Records, Patients |
| Robotic Vacuum          | IR Sensors, Cameras   | Wheels, Suction     | Home, Floors              |

---

## **Key Takeaways**
1. **Agents** use sensors to perceive the environment and actuators to perform actions.
2. **Percept Sequence**: The entire history of percepts received by the agent.
3. **Rationality**: The concept of rational agents is based on their ability to take actions that maximize performance, given what they perceive and know.
4. **Agent Design**: Agents are implemented as programs running on physical architectures.

This section establishes the fundamental relationship between agents and their environments, laying the groundwork for designing intelligent systems.

