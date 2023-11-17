# 8. Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.
## Equipment’s required:
Visual Components Premium 4.3
## Procedure:
1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.
## Program
```
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)
```
## Output
### 1. Generic Articulated Robot
![280909325-af92e9ca-b3bb-4f46-8a0a-7e5207b0e76f](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/31417441-9576-4a78-a04a-ebcce4902dfc)
### 2. robot.driveJoints(0,0,0,0,0,0)
![280909384-3838686b-cc2e-4460-9757-75d6f2d5c366](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/9480cdc1-f2d3-4210-abd0-27ace25f3bca)
### 3. Movement of Joint1
![280909438-573a3295-f5c0-4373-90ce-03e1bcf2b798](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/262b9fde-874c-49c9-8daa-dfc53a509a81)
### 3. Movement of Joint2
![280909488-8b804be2-03cd-432d-99f3-d953001ca00e](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/c099b932-bf3b-4df3-9ec3-f3c9d28799f4)
### 3. Movement of Joint3
![280909520-d8ffe31e-a088-42b1-a026-87eb1d14a801](https://github.com/Darkwebnew/Movement-of-Robot-Joints/assets/143114486/ce203c1f-da82-4d9e-aa80-8c43dd82df81)
## Result 
Thus the different robots joints are moved with the help of python list.
