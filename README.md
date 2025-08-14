# C64SpriteEditor
An on system C64 sprite editor in BASIC and assembly.


Summary of Sprite Editor Commands
-------------------------------------------------------------------------------
Cursor Keys    Navigate around the editor window  

HOME			     Returns the cursor to the top left  

SHIFT HOME		 Clears the editor window  

L/R/U/D		     Move the sprite one pixel left,right,up,down  

-/+			       Cycle through colors for selected pen  
SHIFT B		     Cycle the background color  
SHIFT M		     Toggle between single and multicolor modes  
SHIFT X		     Toggle horizontal expansion of sprite preview  
SHIFT Y		     Toggle vertical expansion of sprite preview  
SHIFT H		     Flip the sprite horizontally  
SHIFT V		     Flip the sprite vertically  
SHIFT S		     Save the sprite to a binary file  
SHIFT L		     Load a sprite into the editor from a binary file  
F8			       Export the sprite as DATA statements to a new BASIC program  
F2			       Change the address value in the header of the sprite binary file  
SHIFT Q		     Quit the C64 Sprite Editor  
  
  
Example of using Sprite from DATA statements  
-------------------------------------------------  
10 FOR T=0 TO 62:READ A:POKE 832+T,A:NEXT  
20 POKE 53269,1:POKE 2040,13  
30 POKE 53248,160:POKE 53249,160  
1000 DATA 0,0,0,0,0,0,0,0  
1010 DATA 0,0,0,0,0,0,0,0  
1020 DATA 0,0,15,240,0,29,184,0  
1030 DATA 57,140,0,49,143,248,127,255  
1040 DATA 252,127,255,254,235,255,174,221  
1050 DATA 255,118,28,0,112,8,0,32  
1060 DATA 0,0,0,0,0,0,0,0  
1070 DATA 0,0,0,0,0,0,0  
