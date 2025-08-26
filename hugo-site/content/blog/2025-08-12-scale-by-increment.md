---
title: test mermaid
date: 2025-08-12T10:00:00+09:00
draft: false
slug: notion-embed
---

## FlexSim configuration overview

This diagram shows how configuration files point to the FlexSim executable and how the validation logic checks for its existence.

```mermaid
flowchart TD
  subgraph Config[Configuration Files]
    A["HelloWorld/paths.py:3"]
    B["Elevator/paths.py:3"]
    C["PickingModel/paths.py:3"]
  end

  subgraph FlexSim[FlexSim Installation]
    F["C:/Program Files/FlexSim 2024/program/flexsim.exe"]
  end

  subgraph Validation[Validation Logic]
    V["os.path.exists(flexsim)"]
  end

  A --> F
  B --> F
  C --> F
  F --> V

  style Config fill:#111827,stroke:#374151,stroke-width:1px,color:#ffffff
  style FlexSim fill:#0b1220,stroke:#374151,stroke-width:1px,color:#ffffff
  style Validation fill:#111827,stroke:#374151,stroke-width:1px,color:#ffffff
```

Notes:
- Replace the executable path with your actual FlexSim install path if different.
