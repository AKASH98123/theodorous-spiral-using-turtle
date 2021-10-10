# theodorous-spiral-using-turtle


import math
import turtle
a=turtle.Turtle()
b=turtle.Screen()
a.speed(10)
b.bgcolor("black")
a.color("red","white")
x=100
y=100

for _ in range(16):
    
    q=math.sqrt(x**2+y**2)
    
    a.fd(x)
    if x==y:
        a.lt(90)
        a.fd(y)
    
    d=math.degrees(math.atan(x/y))
    a.lt(90+d)
    a.fd(q)

    a.bk(q)
    a.rt(90)
    
    y=q
    
