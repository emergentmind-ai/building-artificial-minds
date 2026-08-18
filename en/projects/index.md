---
layout: default
title: Projects
language: en
permalink: /en/projects/
---

# Projects

## SwarmMind

SwarmMind is a simulation project exploring how a swarm of simple, autonomous agents can organize itself into a temporary intelligent system capable of learning and performing task-specific behavior.

The central idea is to treat intelligence not as something that has to be implemented inside a single artificial agent, but as something that can emerge from the organization and interaction of many simple agents. Each individual protozoan in SwarmMind has only limited capabilities. It can perceive aspects of its local environment, communicate with nearby agents, establish physical connections, and modify its behavior. Intelligence emerges when these agents organize themselves into larger functional structures.

This raises a fundamental question: **How can a swarm of individually limited agents form the computational and physical organization required to perform a specific task—and subsequently reproduce that organization and what it has learned when the task occurs again?**


### From swarm to intelligent structure

A swarm initially exists as a collection of independent protozoa with no predefined organization. When a task is introduced, environmental signals guide the swarm toward a structure suited to that task. Task-specific pheromones provide spatial information that allows individual protozoa to recognize where they should position themselves and how the overall structure should form.

The resulting structure is not merely a physical arrangement. It also forms an embedded computational network. Protozoa occupying different positions within the structure assume different functional roles, forming input, processing, and output layers. Connections between neighboring protozoa become weighted communication pathways, allowing sensory information to propagate through the structure and ultimately produce coordinated actions.

The physical structure therefore serves two purposes simultaneously. It provides the mechanical organization required to perform the task, while also providing the spatial topology within which the swarm's computational network operates.

This creates a fundamental difference from a conventional artificial neural network. A conventional neural network is normally defined first as an abstract computational structure and then executed on fixed hardware. In SwarmMind, the computational structure itself is embedded in a population of physical agents. The network must first organize itself within the swarm, and the agents implementing the network can subsequently separate and reorganize.


### Transient neural networks

One of the central challenges of SwarmMind is that the neural network is not permanent.

The protozoa are not fixed neurons occupying permanent positions. They are independent agents that may participate in different structures at different times. When a task is completed, the structure can dissolve and the protozoa return to the swarm. When the same task is encountered again, a new structure must be established.

Consequently, SwarmMind requires a mechanism for preserving the knowledge acquired by a task-specific structure after that structure has dissolved, so that it can be reconstructed within a newly formed structure when the task occurs again.

The current approach therefore separates the learned network from the identities of the individual agents. Once a task-specific structure forms, a distributed mechanism establishes the functional roles of the protozoa and propagates the previously learned connection weights through the newly formed structure. A centrally identified protozoan provides the starting point for this propagation, allowing the network to be reconstructed from the inside outward without requiring the new formation to reproduce the exact geometry of a previous one.

What must be preserved is not the identity or position of individual protozoa, but the functional organization of the task-specific network. When the task occurs again, this organization must be mapped onto the newly formed physical structure, even if its geometry and the individuals participating in it differ from the previous formation.


### Intelligence embedded in morphology

The neural network is only one part of the system. Its output must ultimately influence the physical structure of the swarm.

For example, the current case study investigates jellyfish-inspired locomotion. Protozoa at the outer rim of the structure interact directly with the environment. Those at the sensory region collect information such as pheromone concentrations, water flow, and other environmental properties. This information enters the internal neural network, is processed through the hidden layers, and reaches output protozoa at the opposite side of the structure.

The output protozoa act as actuators. Their coordinated activity generates forces through the connected structure, causing it to deform and move in a coordinated manner and thereby propel the jellyfish-like swarm through the surrounding fluid.

The morphology of the swarm is therefore part of the computational system. The arrangement of the agents determines which agents can communicate, which agents can sense the environment, and which agents can physically influence it. Conversely, the behavior produced by the neural network changes the physical state of the swarm and its environment.

This creates a feedback loop between computation, morphology, and environment.


### From a jellyfish to task-specific morphology

The jellyfish structure is deliberately used as a concrete case study rather than as the final objective of SwarmMind.

The broader goal is to investigate whether the same principles can support different task-specific structures. A task requiring locomotion might produce a compact, coordinated structure. A task requiring reaching might produce elongated or tentacle-like extensions. Other tasks could require different spatial organizations and different internal computational networks.

The swarm should therefore not be understood as a fixed organism with a predefined body plan. Instead, its morphology should emerge from the task it is required to perform.

This leads to a fundamental concept underlying SwarmMind: **the physical structure of the intelligent system is itself adaptable**.


### Swarm and brain

This perspective also provides a different way of thinking about the relationship between swarm intelligence and individual intelligence.

A brain is not an indivisible computational entity. Its intelligence emerges from a large population of relatively simple cells whose interactions form complex, distributed networks. Individual neurons do not possess the intelligence of the organism. Intelligence emerges from their organization and interaction.

A swarm can be viewed in a similar way. Its individual protozoa need not be intelligent in isolation. Instead, intelligence can emerge from the temporary organization of many agents into functional networks.

The important difference is the persistence of the connections. Neural networks in biological brains maintain relatively stable physical structures, while a swarm can continuously dissolve and recreate its connections.

This shifts the central question from whether a distributed system can be intelligent to a more specific problem:

**How can useful intelligence persist when the physical network that implements it is constantly changing?**

SwarmMind investigates this question by treating structure formation, neural-network formation, learning, memory, and physical action as parts of the same system rather than as separate mechanisms.


### A simulation for exploring the mechanisms

SwarmMind is intended primarily as an experimental simulation framework for investigating these mechanisms.

The current jellyfish case study provides a controlled environment in which the complete process can be explored: a loose swarm receives a task-specific signal, forms a task-appropriate structure, establishes an internal neural network, assigns functional roles, applies or learns connection weights, interacts with its environment, performs the task, and eventually dissolves. When the task occurs again, the swarm should be able to reconstruct the required organization and reuse what it has previously learned.

The purpose of this approach is not to reproduce a biological organism in every detail. Instead, biological principles such as swarm organization, environmental signaling, physical connectivity, distributed computation, and adaptive morphology provide mechanisms from which an artificial system can be constructed.

SwarmMind therefore explores a broader question:

**Can a collection of simple agents become an intelligent system by dynamically organizing themselves into the computational and physical structure required for the task at hand?**

<!--
---



There are also three conceptual points I would preserve very carefully in the project going forward:

1. **The neural network is not the whole intelligence.** It is the computational component of a larger system involving morphology, sensing, actuation and environment.
2. **The structure is not merely an output of intelligence.** It is also part of the mechanism that makes the intelligence possible. The topology determines communication, sensing and action.
3. **The real research problem is transient intelligence.** The interesting question is not simply whether a swarm can learn, but whether it can **reconstruct a functional organization after its previous physical organization has disappeared**.
-->
