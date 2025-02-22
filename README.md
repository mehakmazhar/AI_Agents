# AI_Agents
An intelligent agent (IA) is an entity that makes a decision that enables artificial intelligence to be put into action. It can also be described as a software entity that conducts operations in the place of users or programs after sensing the environment. It uses actuators to initiate action in that environment.

# How intelligent agents work
Intelligent agents work through three main components: sensors, actuators, and
effectors. Getting an overview of these components can improve our understanding of
how intelligent agents work.
**Sensors**: These are devices that detect any changes in the environment. This
information is sent to other devices. In artificial intelligence, the environment of
the system is observed by intelligent agents through sensors.
**Actuators:** These are components through which energy is converted into
motion. They perform the role of controlling and moving a system. Examples
include rails, motors, and gears.
**Effectors:** The environment is affected by effectors. Examples include legs,
fingers, wheels, display screen, and arms.

![image](https://github.com/user-attachments/assets/7e5e6cde-1d0b-45b9-a796-b32b2bc1b80f)

# Examples of Agents
- A Software agent 
- A Robotic agent

# Relating AI-Based Agents to Human Behavior
Artificial Intelligence (AI) agents are designed to mimic human decision-making
processes, often drawing parallels with how people act and respond in daily life. Reflex
agents in AI, like humans' instinctive reactions, respond immediately to stimuli without
deeper thought, such as an automated braking system in cars that stops when an
obstacle is detected. Model-based agents use stored knowledge to make informed
decisions, similar to how people rely on experience, like checking the weather before
dressing for the day. Goal-based agents are comparable to humans setting objectives
and taking steps to achieve them, such as planning a trip or saving for a vacation.
Utility-based agents evaluate multiple factors to optimize outcomes, just as individuals
balance cost, quality, and convenience when choosing products or services. Lastly,
learning agents improve performance over time by gathering feedback, much like
humans learn from mistakes and experiences to refine their skills. This relationship highlights how AI systems emulate human cognitive functions to solve problems,
automate tasks, and enhance decision-making in real-world applications.

# Real-World Behaviors Reflecting AI Agent Principles
**1. Reflex Agent (Immediate, automatic responses)**
Pulling your hand away after touching a hot object.
Blinking when something moves rapidly toward your face.
Ducking when a ball is thrown unexpectedly at you.
Swerving your car to avoid an obstacle on the road.
Sneezing when exposed to dust or allergens.
**2. Model-Based Agent (Using past knowledge to inform decisions)**
Looking outside or checking the weather app before dressing for the day.
Turning on headlights when driving in a tunnel because you know it will be dark.
Remembering a store’s layout to quickly find an item on a return visit.
Closing windows when it starts to rain based on previous experiences.
Adjusting room temperature by using the thermostat when feeling cold or hot.
**3. Goal-Based Agent (Actions aimed at achieving specific goals)**
Planning a study schedule to pass an upcoming exam.
Organizing a shopping list to save time and avoid unnecessary purchases.
Mapping a route to reach a new location efficiently.
Scheduling workouts to achieve fitness goals.
Saving money for a specific purpose, like a vacation or a car.
**4. Utility-Based Agent (Maximizing overall satisfaction or utility)**
Choosing between two jobs by considering salary, location, and work-life
balance.
Selecting a phone by weighing features like camera quality, battery life, and
price.
Picking a restaurant based on food quality, ambiance, and cost.
Deciding which movie to watch by balancing reviews and your mood.
Choosing between walking or driving based on distance, time, and weather
conditions.
**5. Learning Agent (Improving actions based on feedback)**
Learning to bake a cake better after receiving feedback from previous attempts.
Adjusting study techniques after noticing which methods improve test scores.
Refining a presentation style after audience feedback.
Improving navigation skills after getting lost and finding a better route.
Learning a new language through practice and correcting mistakes over time.

# Working of Agents
When designing any intelligent agent system, it is essential to create three main
components:
**1. The Environment:**
○ The external system with which the agent interacts. It provides percepts
(sensory inputs) and responds to the agent’s actions.

```python
class Environment:
    def __init__(self, initial_state):
        self.initial_state = initial_state  # Initial state could be fixed or random

    def get_percept(self):
        # Initial condition of environment, that would be perceived by agent
        pass
```

**2. The Agent:**
○ The decision-making entity that perceives its environment and takes
actions to achieve a goal.

```python
class SimpleReflexAgent:
    def __init__(self):
        pass

    def act(self, percept):
        # Determine action based on the initial percept
        pass
```
**3. The Agent Program:**
○ The internal mechanism that determines the actions the agent takes
based on its precepts.

This interaction allows the agent to move within the environment and perform its
functions effectively. The following example demonstrates these components with a
simple reflex agent.

```python
def run_agent(agent, environment):
    # The agent reacts to the initial stimulus/Percept
    percept = environment.get_percept()
    action = agent.act(percept)
    print(f"Percept: {percept}, Action: {action}")

# Create instances of agent and environment
agent = SimpleReflexAgent()
environment = Environment(initial_state=0)  # Start with any
# initial condition (high/low, 1/0, True/False, high/med/low etc. based on scenario)

# Run the agent in the environment (only once)
run_agent(agent, environment)
```


