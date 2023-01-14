# Test 

# Firewall Rules
```mermaid
graph TD
  classDef sgi fill:#0000cc,stroke:#0000cc,stroke-width:4px;
  classDef sge fill:#009000,stroke:#009000,stroke-width:4px;


  SGe-Internet:::sge -- SSH,DNS,tcp-443 --> SGi-bastion:::sgi

```

# Definition SecurityGroups (graph)

```mermaid
graph TB;
  classDef sgi fill:#0000cc,stroke:#0000cc,stroke-width:4px;
  classDef sge fill:#009000,stroke:#009000,stroke-width:4px;

  subgraph one
    SGe-Internet(SGe-Interne<hr><table><tr><td>ip</td><td>all</td></tr><tr><td>tag</td><td>sectagname</td></tr></table>):::sge
  end

  subgraph two
    SGe-secgroup01(SGe-secgroup01<hr><table><tr><td>ip</td><td>all</td></tr><tr><td>tag</td><td>sectagname</td></tr></table>):::sge
    SGe-secgroup02(SGe-secgroup02<hr><table><tr><td>ip</td><td>all</td></tr><tr><td>tag</td><td>sectagname</td></tr></table>):::sge
  end

```

# Definition SecurityGroups (erDiagram)
```mermaid
%%{init: {'themeCSS': '.er.entityBox { fill: #0000cc; } .er.attributeBoxOdd { fill: #0000cc;} .er.attributeBoxEven { fill: #0000cc;} ' }}%%

erDiagram

  SGi-bastion {
    VM bastion
    SecTag Tag
  }
  
  SGi-secgroup01 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup02 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup03 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup04 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup05 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup06 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup07 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup08 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup09 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup10 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup11 {
    VM bastion
    SecTag Tag
  }

  SGi-secgroup12 {
    VM bastion
    SecTag Tag
  }  

```

# Definition IPSets

```mermaid
%%{init: {'themeCSS': '.er.entityBox { fill: #009000; } .er.attributeBoxOdd { fill: #009000;} .er.attributeBoxEven { fill: #009000;} ' }}%%

erDiagram 
  SGe-Internet {
    IP all
    Tag tag
  }
  
```