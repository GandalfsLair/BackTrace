# BackTrace
A program to emulate being traced. Think Sneakers-NSA-Phonecall and you have it 

** What is it? **
If you have seen any hacking movie then you know there is usually a sequence where the hacker is being traced. 
This is shown a number of different ways, but the most common is the map with the red line getting closer to the Hacker. 
Added tension is created via a beeping that gets quicker and faster... 

I have not added the sound to this...

But in essence this is a program that takes an image of a map, overlays a workspace onto the image, then plots points 
into this workspace. Hitting space bar makes the line track back to the next point.

** Using a Different Map **
Save the new image file into the same location as the BackTrace program.
Maybe this is a city map? Maybe its a plan of satellites in orbit? Who knows. 

** Adding extra points **
Find the section of the code marked Const Nodes = {
Copy and paste extra lines at the bottom of the list. 
The current version has 5 hops (meaning 6 locations total - The Start, the End, and 4 Relay Points)
If you add more ensure you put a comma at the end of the line!!
The starting point of the trace goes at the top. The location of the hacker goes at the bottom. 

Assuming this is being used in a modern day game on planet Earth I have enclosed as comments in the code 
the coordinates of a number of cities. These are pretty rough... feel free to edit and amend.

** Coordinated for New Maps **
The coordinate system is based on the size of the image. 
The map of Planet Earth that is attached to the code is 800 pixels by 500 pixels 
Therefore the centre of the map is at 400 by 250

Adding a new map requires you to know the size of the image (this can be found by looking at the properties of the image.)
New coordinate are therefore calculated with the new size in mind. 
X = Horizontal Axis
Y = Vertical Axis

** Making the Trace **
Hitting the SPACE BAR triggers the tracing. 
For each press of Space, the next section of the track is highlighted Blue. 
This can be changed in the CSS (See the section .signal )

Currently there is no special activity when the final node is reached. 
This could be amended in future versions.


** Legally Bits  **
This is not my strong point. I am likely to mess this up.
My intention is to release this so that you can take it, use it, copy it, amend it, and improve on it.
If you do improve on it, please let me know!!

As such I attach the following Open Source Statement;

Copyright (c) [2025] [Dave Ingham]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

The Map Image that comes with this program was located at :- https://t3.ftcdn.net/jpg/04/43/26/18/360_F_443261883_26RpFwpdz87VMOWX2zrrHxOrBlmKw1DA.jpg
I do not own or have any claim on this image. 
If I have done anything wrong by taking a copy of this image I apologise. This was not my intention. Again, please let me know and I can remove the image if needed. 

