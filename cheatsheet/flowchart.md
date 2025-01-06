# Flowchart Guide

Flowcharts are used to represent workflows, processes, and decision trees.

## Basic Syntax

```mermaid
graph TD
    A --> B
    B --> C
    C --> D
```

## Node Shapes

```mermaid
graph TD
    A[Rectangle]
    B(Rounded Rectangle)
    C([Stadium shape])
    D[[Subroutine]]
    E[(Database)]
    F((Circle))
    G>Asymmetric]
    H{Diamond}
    I{{Hexagon}}
    J[/Parallelogram/]
    K[\Parallelogram alt\]
```

## Arrow Types

```mermaid
graph LR
    A --> B    %% Basic arrow
    C ==> D    %% Thick arrow
    E -.-> F   %% Dotted arrow
    G ==> H    %% Thick arrow
    I --- J    %% Line without arrow
    K o--o L   %% Circle connections
    M x--x N   %% Cross connections
```

## Subgraphs

```mermaid
graph TB
    subgraph one
        a1 --> a2
    end
    subgraph two
        b1 --> b2
    end
    a1 --> b2
```

## Direction

- TB - top to bottom
- TD - top-down (same as TB)
- BT - bottom to top
- RL - right to left
- LR - left to right

## Styling

```mermaid
graph LR
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
    
    style A fill:#f9f,stroke:#333,stroke-width:4px
    style B fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
```

