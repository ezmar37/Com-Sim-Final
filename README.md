# Computer Simulations Final Project

### Agent-Based Simulation of Prescription Pain Reliever Misuse
This repository contains an agent-based simulation exploring how access to mental health resources and rehabilitation services influences community-level prescription pain-reliever misuse. The project integrates **real-world survey data** with **computational modeling** to understand the impact of inclusive resources on substance-use outcomes.



### Dataset  
We used the publicly available **Predicting Pain Reliever Misuse / Abuse** dataset from Kaggle:
https://www.kaggle.com/datasets/thedevastator/predicting-pain-reliever-misuse-abuse/data

The dataset is derived from NSDUH (National Survey on Drug Use and Health) indicators and includes variables for:
- Prescription pain-reliever misuse  
- Age, sex, mental health indicators  
- Illicit drug use (heroin, cocaine, amphetamines, etc.)  



---
### Project Structure

#### Agent-Based Simulation 🤖 

Each individual in the dataset becomes a simulated **agent** with the following attributes:

- Age category  
- Sex  
- Mental health distress score  
- Prior pain-reliever misuse  
- Other drug involvement (heroin, cocaine, amphetamine)  
- A computed baseline probability (`p_base`) of misuse  


We simulated two communities:

##### 1. Baseline Scenario (No Added Resources)  
   Agents maintain their baseline misuse risk over time.

##### 2. Inclusive Resources Scenario  
   High-risk agents have a chance to receive:
   - Mental health support  
   - Rehabilitation services  

Rehab exposure reduces an agent’s misuse probability using an exponential decay function.  

#### Dataset Misuse Analysis
After the simulation, we visualized the dataset to understand misuse patterns across drug categories.  
This step is *independent from the agent-based simulation* and does **not** affect agent behavior.

