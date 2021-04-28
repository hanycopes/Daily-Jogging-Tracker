README.md

# TL;DR

1. A simple GUI using Kivy to keep track of daily habits

1. Daily habits might include finances,exercise,meditation,learning languages,

and all kinds of different habits you'd like to have.


# TODO: 

[x] Spawn a new window when a button is pressed

[_] Look for some resource about timers that use Kivy

[_] Fix navigation 


# Process:

[_] Learn about basic Kivy 

[_] Creating a .kv File

[_] The first thing we need to do to add widgets to our screen using .kv is set up an empty class in our python script.

[_] Two important things to remember about .kv files:
- Capitals are Important
- Indentation is important

[_] To set up object properties we need to create global variables from within our .kv file and assign these variables to the id property of specific widgets.

[_] .kv file basics :
        [_] TextInput:

        [_] Label:

        [_] Button:
            
            [_] pos_hint = {"x":1, "y":1, "left":1, "right":1, "top":1, "bottom":1}

            [_] we can change the properties based on the state of the button

            [_] Floatlayout; define properties without having to repeat them

            [_] - pos_hint

                - size_hint
                Note 1: You can only use values between 0-1 for both size_hint and pos_hint. Where 0 = 0% and 1 = 100%.

                Note 2: The coordinate system  in kivy works from the bottom left! This will be important when placing our objects.     

[_] Floatlayout:
        A FloatLayout allows us to place elements using something called a relative position. This means that rather than defining specific coordinates we will place everything using percentages or based on the current window width and height.

[_] Handle input from user using Touch Class

[_] on_touch_down, on_touch_up, on_touch_move

[_] Using a Builder for .kv File



# Objectives:

[_] General and deeper understanding of OOP

[_] Creating a GUI that runs on multiple systems

[_] Getting used to classes, functions

# Errors:

[_] https://www.techwithtim.net/tutorials/kivy-tutorial/multiple-screens/

[_] Error:
```[CRITICAL] [Application ] No window is created. Terminating application run.
[INFO   ] [Base        ] Start application main loop
[ERROR  ] [Base        ] No event listeners have been created
[ERROR  ] [Base        ] Application will leave``` 
   
[_] Solution:
    from kivy.core.window import Window
