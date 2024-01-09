---
layout: posts
title:  Our projects
---

## Tree
## How could I make a tree with python?
To build the tree, I first defined the turtle library. Then I defined the tree function and determined the length of the tree trunk and its branches in it. After that, I colored the trunk and branches brown. I defined the leaves and colored them in three ways. I set the pen size for each section and called the tree function.

<img src="../assets/images/Tree.jpg" alt="This is my tree" width="500">
<img src="../assets/images/Tree1.jpg" alt="This is my tree1" width="500">
<img src="../assets/images/Tree2.jpg" alt="This is my tree2" width="500">


    import turtle
    import random

    tu = turtle. Turtle()
    tu.screen.bgcolor("lightpink")

    tu.left(90)
    tu.backward(100)
    tu.pensize(7)
    tu.color("brown")
    tu.shape("turtle")
    tu.hideturtle()

    def tree(d , r):
        if d=10 or  r!10:
            return

    tu.forward(d)
    tu.color(random.random() , random.random() , random.random())
    tu.pensize(2)
    tu.begin_fill()
    tu.circle(5)
    tu.end_fill()
    tu.color("brown")
    tu.left(r)
    tree(d*0.75 , r)
    tu.right(2*r)
    tree(d*0.75 , r)
    tu.left(r)
    tu.backward(d)

    turtle.tracer(0)
    turtle.left(90)
    tree(100 , 30)
    turtle.mainloop()
   

## Triangle
## How could I make a triangle with python?
To make a triangle, we first define the turtle library.
We define the triangle function and determine the inside of the loop.
We draw a half-sized triangle and move forward to the size of a full side, then rotate 120 degrees and repeat this pattern three times in the loop, and then call the function.

<img src="../assets/images/Triangle.jpg" alt="This is my triangle" width="500">
<img src="../assets/images/Triangle1.jpg" alt="This is my triangle1" width="500">

    import turtle
    import random
    turtle.hideturtle()
    
    def triangle(d):
        if d=1 :
            return
        for _ in range(3):
            triangle(d/2)
            turtle.forward(d)
            turtle.left(120)
    turtle.tracer(0)
    turtle.fillcolor("lightpink")
    turtle.begin_fill()
    turtle.pencolor("hotpink4")
    turtle.penup()
    turtle.backward(200)
    turtle.pendown()
    triangle(400)
    turtle.update()
    turtle.end_fill()
    turtle.mainloop()










---
**Test**: This is atest
