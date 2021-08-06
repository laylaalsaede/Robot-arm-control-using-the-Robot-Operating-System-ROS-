# Robot-arm-control-using-the-Robot-Operating-System-ROS
This project is one of my projects in AI as an intern in Smart Methods, in this project will create and simulate robot arm using robot operating system (ROS).
# Start a new project 
After creating an account at: https://www.theconstructsim.com website, Must click on "create new project" 

Then you have start filling the blanks by choosing the version ROS such as melodic which i used, Then Writing the name of your project and description then click "create" .

Your project will be as shown in the picture:

![2021-08-06](https://user-images.githubusercontent.com/63214056/128528411-5fba8aa7-377c-4e23-90ce-d880492da6df.png)

Click Run and then wait for a while for this interface shown:

![2021-08-06 (2)](https://user-images.githubusercontent.com/63214056/128530384-f7665d1f-7f59-44e5-bfb0-9c6b605febe0.png)


# Installing the package arduino_robot_arm & dependencies
Firstly, Open the "shell web"

Then use the commands:

 - Add the “arduino_robot_arm” package to “src” folder :
 
	   $ cd ~/catkin_ws/src
	
	   $ sudo apt install git
	
	   $ git clone https://github.com/smart-methods/arduino_robot_arm 
  
- Install all the dependencies :

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


# Controlling the motors
Now will run the robot arm packge using this command ($ roslaunch robot_arm_pkg check_motors.launch ) the click on graphical tools which will open the window show the simulate arm , as shown in the picture :

![2021-08-06 (7)](https://user-images.githubusercontent.com/63214056/128543141-283717ce-6117-4a38-9f6c-639a50457dbf.png)

![2021-08-06 (8)](https://user-images.githubusercontent.com/63214056/128543139-a317c538-54aa-4499-aecd-816d00bfdb07.png)


  
# Controlling the motors in simulation 
This commands will run the arm simulation on RVis and Gazebo 

    $ roslaunch robot_arm_pkg check_motors.launch

    $ roslaunch robot_arm_pkg check_motors_gazebo.launch

    $ rosrun robot_arm_pkg joint_states_to_gazebo.py

As shown in the pictures :

![2021-08-06 (9)](https://user-images.githubusercontent.com/63214056/128543671-3dfc60b7-a844-4c25-862b-cf4d1cf22077.png)
![2021-08-06 (10)](https://user-images.githubusercontent.com/63214056/128543673-5c8f452e-7167-4951-806c-b447784f23b1.png)
![2021-08-06 (11)](https://user-images.githubusercontent.com/63214056/128543666-97a1a8bb-64a7-4ac8-a471-fbe01b5cc1fa.png)

Then click in the gazebo at below the window:

![2021-08-06 (14)](https://user-images.githubusercontent.com/63214056/128543719-7abb873f-7982-41dd-8e0c-ccc3e9fee848.png)


# Movelt in Rvis 
To define the positioning and movements of the arm will using movelt which is simulate the arm movement in different directions, By Using this command ($ roslaunch moveit_pkg demo.launch), As shown in the pictures : 

![2021-08-06 (15)](https://user-images.githubusercontent.com/63214056/128544182-3180d73f-77e9-4530-814f-af55a79b982e.png)
![2021-08-06 (16)](https://user-images.githubusercontent.com/63214056/128544183-f3bd13db-2478-4bb3-91e0-d6a91859fc33.png)


## 📝 Sources 

- [Smart Methods Presentation](https://docs.google.com/presentation/d/1PakayQR6GGvXmXoLaYF_20ktKC39BTSc/edit#slide=id.p30)
- https://github.com/Aqlaa29/Robot-Arm-Project

 
 



