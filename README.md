# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
Developed by: R.Sanjith
RegisterNumber: 212223230191 
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)
```
## Output
### 1. Generic Articulated Robot
![image](https://github.com/sanjithbro/Movement-of-Robot-Joints/assets/167451460/b417a35a-94aa-4fac-9a33-afad9f9819eb)

### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/sanjithbro/Movement-of-Robot-Joints/assets/167451460/77a39b70-9c6a-4d83-97f4-e75610e024c9)

### 3. Movement of Joint1
![image](https://github.com/sanjithbro/Movement-of-Robot-Joints/assets/167451460/e5824624-295d-456d-b452-d67ba3790989)

### 4. Movement of Joint2
![image](https://github.com/sanjithbro/Movement-of-Robot-Joints/assets/167451460/4f129d01-0995-4a79-9d95-5e0aa096d818)

### 5. Movement of Joint3
![image](https://github.com/sanjithbro/Movement-of-Robot-Joints/assets/167451460/f11a6a8f-f38c-4723-993f-1c137de055e3)

## Result 
Thus the different robots joints are moved with the help of python list.


