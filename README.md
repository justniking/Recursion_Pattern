# Recursion_Pattern
from turtle import *

speed(0)
bgcolor("floralwhite")
pensize(1)

colors = ["hotpink", "orange"]

for i in range(36):  # Outer loop for the circular pattern
    pencolor(colors[i % len(colors)])  # Change the pen color
    for j in range(8):  # Inner loop for the original pattern
        left(45)
        for k in range(8):
            forward(100)
            right(45)
    right(10)  # Rotate the entire pattern by 10 degrees

hideturtle()

