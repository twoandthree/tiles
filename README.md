from DrawingPanel import *

import random

"""
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!!!!!!!!!!!!!!!!DO NOT EDIT BETWEEN THESE COMMENTS!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
"""
from DrawingPanel import *

p = DrawingPanel(500, 500)

def main():
    color_value = random.randint(0, 255)
    color = color_value, color_value, color_value
    
    xpos = random.randint(0, 240)
    ypos = random.randint(0, 140)
    
    rect_width = random.randint(25, 60)
    rect_height = random.randint(25, 60)
    
    p.fill_rect(xpos, ypos, rect_width, rect_height, color)

    p.window.bind("<Button-1>", raises)
    p.window.bind("<Button-3>", lower)
    p.window.bind("<Button-2>", lower)
    p.window.bind("<Shift-Button-1>", delete)
    p.window.bind("<Shift-Button-3>", delete_all)
    p.window.bind("<Shift-Button-2>", delete_all)
    p.window.bind("<s>", shuffle)
    p.window.bind("<n>", add)
    add_all()
    draw_all()

"""
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!!!!!!!!!!!!!!!!DO NOT EDIT BETWEEN THESE COMMENTS!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
"""
def add(event):
    #TODO: Called when the user presses n. Adds a tile to the top of the list
    pass

def add_all():
    #TODO: Called when the program starts. Adds 50 tiles (as described in add)
    #to the list of tiles
    pass

def draw_all():
    #TODO: Called when the program starts. Draws all of the tiles in the list on
    #the DrawingPanel. Each tile should have a solid background color and
    #a black outline around it. Tiles should be drawn from the bottom (
    #start) to the top (end) of your list
    pass

def raises(event):
    #TODO: Called when the user left-clicks. The event parameter contains the
    #coordinates where the user clicked. If these dinates touch any tiles,
    #you should move the topmost of these tiles to the very top (end) of
    #the list.
    pass

def lower(event):
    #TODO: Called when the user right-clicks. The event parameter contains the
    #coordinates where the user clicked. If these coordinates touch any
    #tiles, you should move the topmost of these tiles to the very bottom
    #(beginning) of the list.
    pass

def delete(event):
    #TODO: Called when the user Shift-left-clicks. The event parameter contains the
    #coordinates where the user clicked. If these coordinates touch any tiles,
    #you should delete the topmost of these tiles from the list
    pass

def delete_all(event):
    #TODO: Called when the user Shift-right-clicks. The event parameter contains the
    #coordinates where the user clicked. If these coordinates touch any tiles,
    #you should delete all such tiles from the list.
    pass

def shuffle(event):
    #TODO: Called when the user types s. This function should move every tile on the
    #screen to a new random x/y pixel position. These positions should follow
    #the same rules as described in add. 
    pass

main()
    
    

    

