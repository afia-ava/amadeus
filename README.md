# Amadeus

- [Introduction](#introduction)

- [System Design](#system-design)

- [Components](#components)

- [CAD Model](#cad-model)

![Amadeus1](/images/electrical-comp1.png)
![Amadeus2](/images/electrical-comp2.png)

## Introduction
Amadeus is an observational AI assistant that learns from you by watching and asking the right questions.

My central thesis is that humans are more helpful assistants because they absorb tacit, implicit knowledge that isn’t explicitly stated during task delegation. For example, if you ask an assistant to book a flight, they may already know whether you’re elderly, able-bodied, or disabled; which airlines you prefer; your location and time zone (so they don’t book a flight at 3 a.m.); your budget; your seat preferences; and many other details. You typically don’t tell an assistant, “I’m disabled,” or even state your location and time zone, because those facts are often inferred or learned through prior interaction. But if you delegate the same task to an AI, it usually won’t perform as well as a human assistant because it lacks reliable mechanisms for capturing that tacit context.

So I’m building an assistant that can become a truly helpful personal AI through active interrogative learning: a multimodal device that passively observes daily life (video, audio, and environmental context) and strategically asks questions to fill knowledge gaps and resolve ambiguity. Rather than merely recording, its purpose is to learn continuously from lived experiences and use that learning to train a personal context graph.


## System Design
The main domain for system domain questions are memory sysrems and knowledge representation. The questions to research further into include:

- How should continuous experience be segmented into episodes?
- What triggers memory consolidation?
- How to represent entities changing over time?

## Components
1. Raspberry Pi 5 Board
2. Raspberry Pi Halio with 13 TOPs
3. Storage
4. Sensors for vision, depth, audio, power
5. CAD model
Details about components can be found in Bill of Materials (BOM) file. 

## CAD model 
I'm planning to model a contrainer with threaded opening so that it's fairly easy to do maintenance if needed. 

3D print CAD model expectations:
- Houses sensors, computer, and a screen/mic array
- It can sit at level fields
- Hole placements for cameras, microphones, sensors, ports
- Airflow/thermal considerations for the compute module (like vent holes/fan mount)
- Fit the Raspberry Pi + HAT + sensors (measure the sizes)
- LED indicator (for status)

I have used some open sourced CAD models in my design to place all the components. All of the models has been sourced from [GrabCAD](https://grabcad.com/library) and [Printables](https://printables.com/). 

I believe this will be a fun and challenging project letting me learn a lot of new skills. If you have any feedback or wisdom to share, feel free to slack me at @afia ava. 
