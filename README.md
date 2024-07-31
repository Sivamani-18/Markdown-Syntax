# Markdown Syntax

This is a comprehensive list of Markdown syntax along with examples for use in your README.md file, including Mermaid diagrams and code blocks for various programming languages.

## Table of Contents

1. [Headings](#headings-syntax)
2. [Lists](#lists-syntax)
3. [Links](#links-syntax)
4. [Images](#images-syntax)
5. [Blockquotes](#blockquotes-syntax)
6. [Inline Code](#inline-code-syntax)
7. [Code Blocks](#code-blocks-syntax)
8. [Tables](#tables-syntax)
9. [Horizontal Line](#horizontal-line-syntax)
10. [Bold and Italics](#bold-and-italics-syntax)
11. [Mermaid Diagrams](#mermaid-diagrams-syntax)


## Headings Syntax
```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

### Example of Headings

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6


## Lists Syntax
**Unordered List:**
```markdown
- Item 1
- Item 2
  - Subitem 2.1
  - Subitem 2.2
- Item 3
```

**Ordered List:**
```markdown
1. First item
2. Second item
3. Third item
   1. Subitem 3.1
   2. Subitem 3.2
```

### Example of Unordered List

- Item 1
- Item 2
  - Subitem 2.1
  - Subitem 2.2
- Item 3

### Example of Ordered List

1. First item
2. Second item
3. Third item
   1. Subitem 3.1
   2. Subitem 3.2

## Links Syntax
```markdown
[GitHub](https://github.com/)
```

### Example of Links
[GitHub](https://github.com/)

## Images Syntax
```markdown
![Image Alt Text](https://via.placeholder.com/150)
```

### Example of Images
![Image Alt Text](https://via.placeholder.com/150)

## Blockquotes Syntax
```markdown
> This is a blockquote.
```

### Example of Blockquotes
> This is a blockquote.

## Inline Code Syntax
```markdown
Inline `code` example.
```

### Example of Inline Code
Inline `code` example.

## Code Blocks Syntax
Add ` ``` ` at the end of all code blocks Syntax.

**JavaScript:**
```markdown
```javascript
function greet() {
    console.log("Hello, world!");
}
greet();
```


**Python:**
```markdown
```python
def greet():
    print("Hello, world!")

greet()
```


**Shell:**
```markdown
```sh
echo "Hello, world!"
```


### Example of Code Blocks
**JavaScript:**
```javascript
function greet() {
    console.log("Hello, world!");
}
greet();
```


**Python:**
```python
def greet():
    print("Hello, world!")

greet()
```


**Shell:**
```sh
echo "Hello, world!"
```

## Tables Syntax
```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1    | Data 1   | Data 2   |
| Row 2    | Data 3   | Data 4   |
```

### Example of Tables
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1    | Data 1   | Data 2   |
| Row 2    | Data 3   | Data 4   |

## Horizontal Line Syntax
```markdown
---
```

### Example of Horizontal Line
---

## Bold and Italics Syntax
```markdown
**Bold Text**
*Italic Text*
***Bold and Italic Text***
```

### Example of Bold and Italics
**Bold Text**
*Italic Text*
***Bold and Italic Text***

### Mermaid Diagrams Syntax
Add ` ``` ` at the end of all mermaid diagrams Syntax.

**Flowchart:**
```markdown
```mermaid
graph TD
    A[Start] --> B{Is it?}
    B -->|Yes| C[Do something]
    B -->|No| D[Do something else]
    C --> E[End]
    D --> E[End]
```

**Sequence Diagram:**
```markdown
```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```

**Class Diagram:**
```markdown
```mermaid
classDiagram
    Animal <|-- Duck
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool is_wild
        +run()
    }
```

**State Diagram:**
```markdown
```mermaid
stateDiagram
    [*] --> Still
    Still --> [*]
    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```

**Entity Relationship Diagram:**
```markdown
```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER {
        string name
        string address
        string phone
    }
    ORDER {
        int orderNumber
        string date
    }
    LINE-ITEM {
        string productCode
        int quantity
        float price
    }
```

**Gantt Chart:**
```markdown
```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2024-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2024-01-12  , 12d
    another task     : 24d
```

**Pie Chart:**
```markdown
```mermaid
pie
    title Key Metrics
    "Sales" : 35
    "Marketing" : 20
    "Development" : 25
    "Customer Support" : 20
```

**Git Graph:**
```markdown
```mermaid
gitGraph
    commit
    commit
    branch develop
    checkout develop
    commit
    commit
    checkout main
    merge develop
    commit
```

### Example of Mermaid Diagrams

**Flowchart:**
```mermaid
graph TD
    A[Start] --> B{Is it?}
    B -->|Yes| C[Do something]
    B -->|No| D[Do something else]
    C --> E[End]
    D --> E[End]
```

**Sequence Diagram:**
```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```

**Class Diagram:**
```mermaid
classDiagram
    Animal <|-- Duck
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool is_wild
        +run()
    }
```

**State Diagram:**
```mermaid
stateDiagram
    [*] --> Still
    Still --> [*]
    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```

**Entity Relationship Diagram:**
```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER {
        string name
        string address
        string phone
    }
    ORDER {
        int orderNumber
        string date
    }
    LINE-ITEM {
        string productCode
        int quantity
        float price
    }
```

**Gantt Chart:**
```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2024-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2024-01-12  , 12d
    another task     : 24d
```

**Pie Chart:**
```mermaid
pie
    title Key Metrics
    "Sales" : 35
    "Marketing" : 20
    "Development" : 25
    "Customer Support" : 20
```

**Git Graph:**
```mermaid
gitGraph
    commit
    commit
    branch develop
    checkout develop
    commit
    commit
    checkout main
    merge develop
    commit
```
