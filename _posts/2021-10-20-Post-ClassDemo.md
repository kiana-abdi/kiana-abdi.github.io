---
layout: posts
title:  Our project
---

## Tree
## How could I make a tree with python?
To build the tree, I first defined the turtle library. Then I defined the tree function and determined the length of the tree trunk and its branches in it. After that, I colored the trunk and branches brown. I defined the leaves and colored them in three ways. I set the pen size for each section and called the tree function.




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
   
---
**Test**: This is atest
