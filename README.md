# sandbox-mermaid
Sandbox for testing Mermaid scripting to draw diagrams. Information on Mermaid can be found [here](https://mermaid.js.org/). Currently working on testing concurrent development of a model and interface.

```mermaid
---
title: Example Git diagram
---
%%{init: { 'logLevel': 'debug', 'theme': 'base', 'gitGraph': {'showBranches': true, 'showCommitLabel':true,'mainBranchOrder': 2}} }%%
gitGraph
  commit
  commit
  branch interface order: 1
  commit
  commit
  checkout main
  commit
  commit
  commit
  checkout interface
  commit
  checkout main
  branch development order: 3
  commit
  commit
  checkout main
  commit
  commit
  merge interface
  
```

# State diagram
Some text to separate the diagrams

```mermaid
---
Test
---
stateDiagram-v2
[*] --> First
    state First {
        [*] --> second
        second --> [*]
    }
```

# Sankey
```mermaid
---
config:
  sankey:
    showValues: false
---
sankey-beta

Hawaii,"Regional CLD",123
Alaska,"Regional CLD",212
Pumped heat,"Heating and cooling, ""homes""",193.026
Pumped heat,"Heating and cooling, ""commercial""",70.672
```

