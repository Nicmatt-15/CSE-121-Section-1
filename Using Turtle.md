# Using Turtle

In this file, we will learn 6 of the common Turtle command that you will use in this class.

---

## Table of Content

- [Start State of Turtle](#start-state-of-turtle)
- [`.forward(...)` Command](#forward-command)
- [`.left(...)` Command](#left-command)
- [`.right(...)` Command](#right-command)
- [`.up()` Command](#penup-command)
- [`.down()` Command](#down-command)
- [`.penColor(...)` Command](#pencolor-command)

---

## Start State of Turtle

When you first create a Turtle Object and run your program, a Turtle will appear in the middle of the screen facing East (right).

![Default Turtle](/img/default_turtle.png)


---

## `.forward(...)` Command

The `.forward(...)` command moves your Turtle towards the direction it's facing leaving a trail of straight line (by default). The command also needs a number (decimal or whole number) inside the pair of parenthesis to specify how far the Turtle should move forward.

Example:

```java
Turtle myTurtle = new Turtle();

myTurtle.forward(100);
```

Output:

![Forward Turtle](/img/forward_turtle.png)

> The Turtle is moving forward to the East because the Turtle faces East (by default) when we first create our Turtle Object.

---

## `.left(...)` Command

The `.left(...)` command turns your Turtle to the left from the direction it's currently facing. The command also requires a number (decimal or whole number) inside the pair of parenthesis to specify the angle the Turtle needs to turn.

Example:

```java
Turtle myTurtle = new Turtle();

myTurtle.left(90);
```

Output:

![Left Turtle](/img/left_turtle.png)

> By default, the Turtle faces East after it is created. Turning the Turtle left 90 degrees causes the Turtle to face North (up).

---

## `.right(...)` Command

The `.right(...)` command turns your Turtle to the right from the direction it's currently facing. The command also requires a number (decimal or whole number) inside the pair of parenthesis to specify the angle the Turtle needs to turn.

Example:

```java
Turtle myTurtle = new Turtle();

myTurtle.right(90);
```

Output:

![Right Turtle](/img/right_turtle.png)

> By default, the Turtle faces East after it is created. Turning the Turtle right 90 degrees causes the Turtle to face South (down).

---

## `.up()` Command

The `.up()` command "lifts" the Turtle up, causing the Turtle to not leave any lines / trail when it moves forward.

This command is useful to reposition your Turtle to another place without accidentally drawing / leaving a line or mark.

Example:

```java
Turtle myTurtle = new Turtle();

myTurtle.up();
myTurtle.forward(100);
```

Output:

![Up Turtle](/img/up_turtle.png)

> Notice that the Turtle does not leave any trail when it's moving forward after the `.up()` command has been executed in the line above.

---

## `.down()` Command

The `.down()` command are generally used in pair with the `.up()` command. After we have sucessfully moved / reposition our Turtle, we can use the `.down()` command to allow the Turtle to start drawing again.

Example:

```java
Turtle myTurtle = new Turtle();

// Moves the turtle to the right without leaving a trail
myTurtle.up();
myTurtle.forward(100);

// Turn Turtle towards North
myTurtle.left(90);

// Start drawing a line to the North 50 pixels long
myTurtle.down();
myTurtle.forward(50);
```

Output:

![Down Turtle](/img/turtle_down.png)

---

## `.penColor(...)` Command

The `.penColor(...)` command allows us to change the color of the Trail that the Turle leaves. The command takes in a String that specifies the color of the trail that the Turtle leaves.

Here are some available color available:

- `"red"`
- `"blue"`
- `"green"`
- `"yellow"`

Example:

```java
Turtle myTurtle = new Turtle();

myTurtle.penColor("red");
myTurtle.forward(100);
```

Output:

![Pen Color Turtle](/img/pencolor_turtle.png)







