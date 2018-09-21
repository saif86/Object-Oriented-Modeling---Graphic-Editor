# Object-Oriented-Modeling
Step-wise procedure to translate a problem statement into class diagram
## Problem Statement
*"Develop a graphic editor that can draw different geometric shapes such as line, circle and triangle. User can select, move or rotate a shape. To do so, editor provides user with a menu listing different commands. Individual shapes can be grouped together and can behave as a single shape."* 

---
### Step 1). Identify Classes
Extract nouns in the problem statement.

Develop a graphic **editor** that can draw different geometric **shapes** such as **line**, **circle** and **triangle**. **User** can select, move or rotate a **shape**. To do so, **editor** provides **user** with a **menu** listing different **commands**. Individual **shapes** can be grouped together and can behave as a single **shape**. 

Eliminate irrelevant classes.
* Editor - Very broad scope
* User – Out of system boundary

Add more classes by analyzing requirements
* Group - required to behave as a shape
  * Individual shapes can be grouped together and can behave as a single shape
* View – editor must have a display area

Following classes have been identified:
* Shape
* Line
* Circle
* Triangle
* Menu
* **Group**
* **View**

![initial](https://user-images.githubusercontent.com/41892175/45860923-6614ff00-bd9c-11e8-87fb-530b0b6dc907.jpg)

---
### Step 2). Identify Associations
Extract verbs connecting objects.

**"Individual shapes can be grouped together"**
* Group consists of lines, circles, triangles
* Group can also consists of other groups

(Composition)

Verify access paths.

**View contains shapes**
* View contains lines
* View contains circles
* View contains triangles
* View contains groups

(Aggregation)

**Menu sends message to View**

(Simple One-Way Association)
### Basic Object Model


