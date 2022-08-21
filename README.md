# Bearing-stick-model
## Bearring
The main purpose of the bearing is to reduce the friction between the joint serfuces
<br/> the main parts of a bearing is :
* inner race
* rolling element
* cage
* outter race
<br/> ![alt text](https://koyo.jtekt.co.jp/en/uploads/column01_03_02.png)
<br/> Here is the design of 18 roller bearing (no need for a cage)
### The design of the inner race 
<br/> The inner race is a simple tube with ( hight=20mm , inner radius=25mm , outter radius=50mm)
<br/> The main challenge was the rollers locations 
<br/> one methd is by using the cloner object
<br/> second method by showing the tube segments & locate it manually 
<br/> third method is by the calculations , since we have 18 roller in symmetric distribution , so the angle between any two adjacent rollers' centers is 360/18=20 , by using the next equations we can find the coordinates , x=sin(n*20) , z=cos(n*20) , y=0 , where n=0,1,....,17
<br/> the last method is by using geometry graphing calculator
<br/> ![alt text](https://github.com/Maashn5/Bearing-stick-model/blob/main/bearing/location%20of%20roller.png)
<br/> Then by creating a cylinder with ( radius=8mm , hight=16mm ) & by using the boole object we can create the hollow for the rollers
<br/> [The stl file for the inner race](https://github.com/Maashn5/Bearing-stick-model/blob/main/bearing/inner%20race%20(ring).stl)
### The design of the roller
<br/> The roller is a simple cylinder with ( radius=7.5mm , hight=16mm )
<br/> But with booling some of the top & bottom surfaces to minimize the friction 
<br/> [The stl file for the roller](https://github.com/Maashn5/Bearing-stick-model/blob/main/bearing/roller.stl)
### The design of the outter race
<br/> The outter race is a simple tube with ( hight=20mm , inner radius=56.5mm , outter radius=62mm)
<br/> [The stl file for the outter race](https://github.com/Maashn5/Bearing-stick-model/blob/main/bearing/outter%20race%20(ring).stl)
### The final bearing
<br/> By assembling all of the above we have the bearing we need
<br/> [The stl file for the bearing](https://github.com/Maashn5/Bearing-stick-model/blob/main/bearing/%E2%80%8F%E2%80%8F%E2%80%8F%E2%80%8Fbearing.stl)
## Stick model
The stick model is like the bones model of the robot
<br/> [The stl file for the stick model](https://github.com/Maashn5/Bearing-stick-model/blob/main/stick%20model/stick%20model.stl)
<br/> We can figure out the angles of the joints by the joint tool 
<br/> by recording the angles before moving the leg 
<br/> ![alt text](https://github.com/Maashn5/Bearing-stick-model/blob/main/stick%20model/Joint0_before.png)
<br/> ![alt text](https://github.com/Maashn5/Bearing-stick-model/blob/main/stick%20model/Joint1_before.png)
<br/> ![alt text](https://github.com/Maashn5/Bearing-stick-model/blob/main/stick%20model/Joint2_before.png)
<br/> by moving the leg 
<br/> ![alt text](https://github.com/Maashn5/Bearing-stick-model/blob/main/stick%20model/Tilted.png)
<br/> then recording the angle again
<br/> ![alt text](https://github.com/Maashn5/Bearing-stick-model/blob/main/stick%20model/Joint0_after.png)
<br/> ![alt text](https://github.com/Maashn5/Bearing-stick-model/blob/main/stick%20model/Joint1_after.png)
<br/> ![alt text](https://github.com/Maashn5/Bearing-stick-model/blob/main/stick%20model/Joint2_after.png)
