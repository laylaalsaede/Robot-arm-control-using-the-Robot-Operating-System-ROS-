# Robot-arm-control-using-the-Robot-Operating-System-ROS
This project is one of my projects in AI as an intern in Smart Methods, in this project will create and simulate robot arm using robot operating system (ROS).
# Start a new project 
After creating an account at: https://www.theconstructsim.com website, Must click on "create new project" 

Then you have start filling the blanks by choosing the version ROS such as melodic which i used, Then Writing the name of your project and description then click "create" .

Your project will be as shown in the picture:

![2021-08-06](https://user-images.githubusercontent.com/63214056/128528411-5fba8aa7-377c-4e23-90ce-d880492da6df.png)

Click Run and then wait for a while for this interface shown:

![2021-08-06 (2)](https://user-images.githubusercontent.com/63214056/128530384-f7665d1f-7f59-44e5-bfb0-9c6b605febe0.png)


# Installing the package arduino_robot_arm 
Firstly, Open the "shell web"

Then use the commands:

 - Add the “arduino_robot_arm” package to “src” folder :
 
	$ cd ~/catkin_ws/src
	
	$ sudo apt install git
	
	$ git clone https://github.com/smart-methods/arduino_robot_arm 
  
- Install all the dependencies :
-  
        	$ cd ~/catkin_ws
	
       $ rosdep install --from-paths src --ignore-src -r -y
	
   	$ sudo apt-get install ros-melodic-moveit
	
	   $ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui
	
	   $ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher
	
	   $ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control
	
- Compile the package

      $ catkin_make

To clone the robot arm package from GitHub by using the path, as shown in the picture :

![2021-08-06 (3)](https://user-images.githubusercontent.com/63214056/128531409-9b7da7cf-cfee-4522-8032-b7368cd471a2.png)

![2021-08-06 (4)](https://user-images.githubusercontent.com/63214056/128531418-2892d80e-2d43-4f68-83cc-f60978569474.png)

![2021-08-06 (5)](https://user-images.githubusercontent.com/63214056/128531424-99a0e53a-71c8-435d-b3fe-5fd54f61cb68.png)



