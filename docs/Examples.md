# Examples

## Mermaid Diagrams

```mermaid
%%{
  init: {
    'theme': 'base',
    'themeVariables': {
        'background': '#fff'
    }
  }
}%%
flowchart LR
    subgraph subgraph1
        direction TB
        top1[top] --> bottom1[bottom]
    end
    subgraph subgraph2
        direction TB
        top2[top] --> bottom2[bottom]
    end
    %% ^ These subgraphs are identical, except for the links to them:

    %% Link *to* subgraph1: subgraph1 direction is maintained
    outside --> subgraph1
    %% Link *within* subgraph2:
    %% subgraph2 inherits the direction of the top-level graph (LR)
    outside ---> top2
```

<!-- tabs:start -->

### **UML Use Case Diagram**

Hello!

### **UML Sequence Diagram**

Bonjour!

### **UML Component Diagram**

Ciao!

<!-- tabs:end -->

## PlantUML Diagrams

```plantuml
@startuml
Alice -> Bob: Authentication Request [[$./other-file docs]]
Bob --> Alice: Authentication Response [[$../other-file docs]]
@enduml
```

```plantuml
@startuml
start
:Hello world;
:This is defined on
several **lines**;
stop
@enduml
```

## Code Blocks

```javascript
// This is a comment
var x = 1;
```
