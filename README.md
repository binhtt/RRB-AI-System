# RRB-AI-System

Formal Event-B models for correctness-preserving rule evolution in Reactive Rule-Based Artificial Intelligence (RRB-AI) systems.

## Overview
This repository provides a refinement-based Event-B framework for modelling reactive rule-based AI systems and analysing correctness preservation under rule evolution.  
The models capture rule execution semantics, safety invariants, and admissible evolution operations such as rule addition, removal, and modification.

The work focuses on safety-critical reactive AI scenarios where rule bases evolve over time while correctness properties must remain preserved.

## Model Structure
The Event-B development follows a layered refinement strategy:

- **RRB-AI-Abstract** — Abstract semantic model of reactive rule execution.
- **RRB_AI_Controller** — Controller-level refinement introducing rule evaluation and enabled rules.
- **RRB_AI_Evolution** — Evolution refinement supporting dynamic rule updates with conflict and redundancy constraints.

Contexts define system states, rules, actions, guards, and evolution constraints.

## Repository Structure
model/
├── context/ # Event-B contexts (.buc)

└── machine/ # Event-B machines (.bum)

docs/
└── figures/ # Architecture diagrams and screenshots

rodin-project/
└── RRB-AI-System.zip # Importable Rodin project (if provided)

## Requirements
- Rodin Platform (Event-B IDE): https://www.event-b.org/

## How to Run
1. Install the Rodin Platform.
2. Import the provided Rodin project archive, or open the machines and contexts manually.
3. Build the project to generate and discharge proof obligations.

## Research Context
These models accompany a research study on invariant preservation under rule evolution in reactive rule-based AI systems, with applications to safety-critical domains such as medical devices and adaptive control systems.

## Citation
If you use this repository in academic work, please cite the corresponding research article (under submission).

## License
MIT License
