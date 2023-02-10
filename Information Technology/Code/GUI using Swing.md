---
modified: Thu 03/11 2022 08:00
---
# GUI Using Swing
#GR10/Q2 #personal/learning 

## Basics
making a frame:
```Java
JFrame frameName = new JFrame("Frame Title");

frameName.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
frameName.setSize(int x, int y);

// rest of code

// Adding Components
frame.getContentPane().add(componentPlacement, componentName);

frameName.setVisible(true);
```

### Component Placement
You can use different layouts to place your components:
- BorderLayout
- FlowLayout
- GridBagLayout

#### Border Layout
![[Border Layout.png]]
#### Flow Layout
![[Flow Layout.png]]
#### Grid Bag Layout
![[Grid Bag Layout.png]]

## Components
Buttons:
```Java
JButton buttonName = new JButton("Button Text");
frameName.getContentPane().add(buttonName);
```

Menu Bar (and menu bar entries)
```java
// Creating the menu bar
JMenuBar menuBar = new JMenuBar();

// Creating Menu Tabs
 JMenu file = new JMenu("File");
 JMenu actions = new JMenu("Actions");
 JMenu help = new JMenu("Help");

// Adding menu tabs to the Menu bar
 menuBar.add(file);
 menuBar.add(actions);
 menuBar.add(help);

// Adding Options to the menu bar

// Adding Menu bar to frame
 frame.getContentPane().add(BorderLayout.NORTH, menuBar);



```