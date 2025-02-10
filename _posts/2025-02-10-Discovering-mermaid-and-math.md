---
# Basic Options
title: Mermaid Diagramming and charting
date: 2025-02-10
categories: [Mermaid, Diagramm, Tutorial, Basics]
tags: [Basic, Mermaid, Data, Analytics, Diagramms, Visualisation, Plotting]

# Additional Options
author: "IronDingo"
pin: true    # pins post to top
math: false   # enables math formatting
mermaid: true # enables mermaid diagrams
image:
  path: "https://avatars.githubusercontent.com/u/57169982?s=200&v=4"
  alt: Mermaid Diagramming and charting tool
--- 


Exploring Mermaid visualisation and math!

### Mermaid

In the Basic Options in the markdown file within the `_posts` folder.
```md
mermaid: true - # Enables Mermaid diagrams for creating flowcharts, like
```
```md
```mermaid
graph TD;
    A-->B;
    B-->C;```
```
gives:
```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop HealthCheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```
```mermaid
pie title NETFLIX
         "Time spent looking for movie" : 90
         "Time spent watching it" : 10
```
```mermaid
  pie title What Voldemort doesn't have?
  "FRIENDS" : 2
  "FAMILY" : 3
  "NOSE" : 45
```
```mermaid
classDiagram
Class01 <|-- AveryLongClass : Cool
Class03 *-- Class04
Class05 o-- Class06
Class07 .. Class08
Class09 --> C2 : Where am i?
Class09 --* C3
Class09 --|> Class07
Class07 : equals()
Class07 : Object[] elementData
Class01 : size()
Class01 : int chimp
Class01 : int gorilla
Class08 <--> C2: Cool label
```

More examples under:
* [Intro https://mermaid.js.org/intro/](https://mermaid.js.org/intro/)
* [Examples https://mermaid.js.org/syntax/examples.html](https://mermaid.js.org/syntax/examples.html)
