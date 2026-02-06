
## Overview
This repository provides a refinement-based Event-B framework for modelling reactive rule-based AI systems and analysing correctness preservation under rule evolution.  
The models capture rule execution semantics, safety invariants, and admissible evolution operations such as rule addition, removal, and modification.

The work focuses on safety-critical reactive AI scenarios where rule bases evolve over time while correctness properties must remain preserved.

### Model Structure
**Contexts**
- **RRB-AI-Abstract** – core abstract sets, guards, effects, and safety invariants
- **RRB_AI_Extended** – rule-conflict and redundancy constraints for evolution

**Machines**
- **RRB-AI-Abstract-Machine** – abstract reactive execution semantics
- **RRB_AI_Controller** – rule evaluation and enabled-rule selection
- **RRB_AI_Evolution** – rule evolution with invariant preservation

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
