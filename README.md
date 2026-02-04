# Amadeus

- [Introduction](#introduction)

- [System Design](#system-design)

## Introduction
Amadeus is an observational AI assistant that learns from you by watching and asking the right questions.

My central thesis is that humans are more helpful assistants because they absorb tacit, implicit knowledge that isn’t explicitly stated during task delegation. For example, if you ask an assistant to book a flight, they may already know whether you’re elderly, able-bodied, or disabled; which airlines you prefer; your location and time zone (so they don’t book a flight at 3 a.m.); your budget; your seat preferences; and many other details. You typically don’t tell an assistant, “I’m disabled,” or even state your location and time zone, because those facts are often inferred or learned through prior interaction. But if you delegate the same task to an AI, it usually won’t perform as well as a human assistant because it lacks reliable mechanisms for capturing that tacit context.

So I’m building an assistant that can become a truly helpful personal AI through active interrogative learning: a multimodal device that passively observes daily life (video, audio, and environmental context) and strategically asks questions to fill knowledge gaps and resolve ambiguity. Rather than merely recording, its purpose is to learn continuously from lived experiences and use that learning to train a personal context graph.


## System Design
The main domain for system domain questions are memory sysrems and knowledge representation. The questions to research further into include:

- How should continuous experience be segmented into episodes?
- What triggers memory consolidation?
- How to represent entities changing over time?

