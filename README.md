# tiles
from DrawingPanel import *
import random

def add():
    pass
    
    
def main():
    p = DrawingPanel(300, 200)
    
    color_value = random.randint(0, 255)
    color = color_value, color_value, color_value
    
    xpos = random.randint(0, 240)
    ypos = random.randint(0, 140)
    
    rect_width = random.randint(25, 60)
    rect_height = random.randint(25, 60)
    
    p.fill_rect(xpos, ypos, rect_width, rect_height, color)
main()

