# Tronijess Architecture

## Overview

Tronijess is a multi-agent system organized around domain-driven design principles. The system is divided into bounded contexts, each with specific responsibilities.

## Bounded Contexts

### Tasks Domain
Coordinates work through task creation, tracking, and dependency management.

### Code Domain
Implements code changes, runs tests, and manages the codebase.

### Learning Domain
Captures knowledge, documents decisions, and maintains architectural understanding.

## Agent Coordination

Agents operate within their domain boundaries and interact through well-defined interfaces:
- Tasks are the primary coordination mechanism
- Domains reference but do not modify other domains' data
- Knowledge flows from Learning to other domains

## Design Principles

1. **Bounded Contexts**: Each domain has clear boundaries and responsibilities
2. **Agent Autonomy**: Agents make decisions within their domain
3. **Knowledge Sharing**: Learning domain provides shared understanding
4. **Task-Based Coordination**: Work is coordinated through explicit tasks

## Future Considerations

This architecture will evolve as we learn more about the system's needs. All significant changes should be documented as ADRs in the `decisions/` directory.
