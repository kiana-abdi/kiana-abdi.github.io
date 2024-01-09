---
layout: posts
title:  Our projects
---

<title>
Making tree , triangle , jungle
</title>

<h1 style="text-align: center; color: rgb(51, 2, 63); background-color: rgba(178, 136, 187, 0.979);">Tree</h1>

<h1 style="text-align: center; color: rgb(1, 150, 33); background-color: rgb(49, 240, 151);">How could I make a tree with python?</h1>

To build the tree, I first defined the turtle library. Then I defined the tree function and determined the length of the tree trunk and its branches in it. After that, I colored the trunk and branches brown. I defined the leaves and colored them in three ways. I set the pen size for each section and called the tree function.

<img src="../assets/images/Tree.jpg" alt="This is my tree" width="500">

<pre>
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
</pre>



<img src="../assets/images/Tree1.jpg" alt="This is my tree1" width="500">

<pre>
    import turtle

    tu = turtle. Turtle()
    tu.screen.bgcolor("light blue")
    tu.pensize(7)
    tu.color("brown")
    tu.left(90)
    tu.backward(100)
    tu.speed(0)
    tu.shape("turtle")
    tu.hideturtle()

    def tree(n):
        if n=10:
            return
        tu.forward(n)
        tu.color("orange")
        tu.pensize(2)
        tu.begin_fill()
        tu.circle(5)
        tu.end_fill()
        tu.color("brown")
        tu.left(30)
        tree(3*n/4)
        tu.right(60)
        tree(3*n/4)
        tu.left(30)
        tu.backward(n)
    turtle.tracer(0)
    
    tree(100)
    turtle.mainloop()
</pre>



<img src="../assets/images/Tree2.jpg" alt="This is my tree2" width="500">

<pre>
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
        tu.color("green3")
        tu.pensize(2)
        tu.begin_fill()
        tu.circle(5)
        tu.color("mediumspringgreen")
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
</pre>
    

   

<h1 style="text-align: center; color: rgb(20, 39, 128); background-color: rgb(168, 235, 247);">Triangle</h1>

<h1 style="text-align: center; color: rgb(146, 20, 72); background-color: rgb(255, 204, 229);">How could I make triangle with python?</h1>
To make a triangle, we first define the turtle library.
We define the triangle function and determine the inside of the loop.
We draw a half-sized triangle and move forward to the size of a full side, then rotate 120 degrees and repeat this pattern three times in the loop, and then call the function.

<img src="../assets/images/Triangle.jpg" alt="This is my triangle" width="500">

<pre>
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
</pre>


<img src="../assets/images/Triangle1.jpg" alt="This is my triangle1" width="500">

<pre>
    import turtle

    t = turtle. Turtle()
    t.screen.bgcolor("purple")
    t.pensize(5)
    t.color("violet")
    t.hideturtle()
    def draw_triangle(t , size):
        t.forward(size)
        t.left(120)
        t.forward(size)
        t.left(120)
        t.forward(size)
        t.left(120)
    def draw_ser(t , n , size):
        if n==0:
            draw_triangle(t , size)
        else:
            draw_ser(t , n-1 , size/2)
            t.forward(size/2)
            draw_ser(t , n-1 , size/2)
            t.left(120)
            t.forward(size/2)
            t.right(120)
            draw_ser(t , n-1 , size/2)
            t.right(120)
            t.forward(size/2)
            t.left(120)
    
    draw_ser(t , 3 , 300)
    turtle.mainloop()
</pre>


<h1 style="text-align: center; color: rgb(136, 43, 1); background-color: rgba(225, 247, 128, 0.979);">Jungle</h1>

<h1 style="text-align: center; color: rgb(2, 87, 59); background-color: rgba(79, 247, 163, 0.979);">How could I make jungle with python?</h1>

To create a forest in Python, you can use the same tree codes and randomly create trees with various sizes and colors. Then we change the background color and our forest is ready.

<img src="../assets/images/Screenshot (61).png" alt="This is my triangle1" width="500">

<pre>
    import random
    import turtle

    tu = turtle. Turtle()

    tu.screen.bgcolor("lightpink")
    tu.left(90)
    tu.pensize(1)
    #tu.color("brown")
    tu.shape("turtle")
    tu.hideturtle()

    def Tree(d, a, w):
        color = tu.pencolor()
        if d < 3:
            return
        if d < 10 and a != 45:
        
            a = 45
            tu.forward(d)
            tu.color("seagreen")
            tu.pensize(2)
            tu.begin_fill()
            tu.circle(7)
            tu.color("mediumspringgreen")
            #tu.color(random.random() , random.random() , random.random())
            tu.end_fill()
            tu.color("orange")
            tu.left(a)
            Tree(d*0.5 , a , w)
            tu.right(2*a)
            Tree(d*0.5 , a , w)
            tu.left(a)
            tu.backward(d)

        tu.pendown()
        tu.pensize(w)
        tu.forward(d)
        tu.left(a)
        Tree(d * (random.random()/2 + 0.4), 
            a * (random.random()/2 + 0.7), 
            w * (random.random()/2 + 0.2))
        tu.right(2 * a)
        Tree(d * (random.random()/2 + 0.4), 
            a * (random.random()/2 + 0.7), 
            w * (random.random()/2 + 0.2 ))
        tu.left(a)
    
        tu.penup()
        tu.backward(d)
        tu.pencolor("salmon4")

    def setup_screen(width, heigh):
        tu.left(90)
        tu.pencolor("green")
        turtle.tracer(0)
        tu.hideturtle()
        turtle.screensize(width, heigh)

    width, height = 1800, 1000
    x=-width/2 + 50
    y=-height/2 + 100
    setup_screen(width, height)
    tree_count = 100
    tu.right(90)
    for ـ in range(tree_count):
        x += random.randint(50, 50)
        y = random.randint(-500, 500)
        tu.penup()
        tu.setpos(x, y)
        tu.pendown()
        Tree(
            random.randint(25, 100), 
            random.randint(5, 50), 
            random.randint(5, 50))
    
    
    

        turtle.update()
        turtle.left(90)

        turtle.mainloop()
</pre>


<img src="../assets/images/Screenshot (62).png" alt="This is my triangle1" width="500">

Three different Jungles...!

<img src="../assets/images/Screenshot (77).png" alt="This is my triangle1" width="500">













---
**Test**: This is atest
