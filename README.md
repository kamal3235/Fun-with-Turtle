# Fun-with-Turtle
# By Abu Kamal
# Draw rectangle on the screen

import turtle
turtle.color("red")
# turtle.pensize(0)  # make line thicker
# turtle.speed(-10)  # change the speed

def back(len):
    turtle.penup()
    turtle.backward(len)
    turtle.pendown()

def square(size):
    for i in range(4):
        turtle.forward(size)
        turtle.left(90)

def triangle(size):
    for i in range(3):
        turtle.forward(size)
        turtle.left(120)

def rectangle(length, height):  #drawing rectangle
    for i in range(2):
        turtle.forward(length)
        turtle.left(120)
        turtle.forward(height)
        turtle.left(60)


square(100)
back(150)
turtle.color("green")
triangle(100)
back(150)
turtle.color("blue")
rectangle(100, 100)
turtle.Screen().exitonclick()
