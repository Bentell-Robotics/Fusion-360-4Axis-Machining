# Fusion 360 4Axis Machining
 Basic 4Axis tools that don't require a paid subscription


Center_Object easily splits a body into multiple bodies and centers them near the origin to prepare for machining. It then flips the bottom part upside-down
If holes are present, use the PrepareHoles script to extend the holes to the top of the stock. Then use PrepareHolesBottom to extend them to the bottom of the stock.
Then both the top and the bottom can be prepared as usual using the manufacturing tab.
Users with 3Axis machines will have to physically flip the part manually.
Users with a 4th axis can use 360_aluminum_freeform.py outside of Fusion 360 to consolidate the post-processed files into a single file that automatically rotates after each side is finished and accounts for horizontal offsets for maximizing stock space and vertical offsets for stock that isn't properly centered (such as flat aluminum extrusions).


On Windows, these folders should be placed under [Username] > AppData > Roaming > Autodesk > Autodesk Fusion 360 > API > Scripts. You can place 360_aluminum_freeform.py wherever you'd like, since it won't be used in Fusion 360.

Before using, please look through the code carefully to confirm that nothing will be damaged using your setup, especially when using 360_aluminum_freeform.py. This was tested on a 3018 CNC router using a 4-chuck 4th axis.
