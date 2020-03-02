This is an example ROS package to accompany chapter 9 of the book Practical Robotics in C++ by Lloyd brombach.


Nodes

Node: got_to_x
Launch the turtlesim_node then launch go_to_x. This simply subscribes to the turtles location, then issues cmd_vel messages to move the turtle to the goal designated as a constant on line 16. 

Subscribed Topics:

/turtle1/pose ([turtlesim::PoseConstPtr])
The turtle's pose



Published Topics
turtle1/cmd_vel ([geometry_msgs::Twist])

Publishes commands (linear.x only) to move the turtle to the constant GOAL




Node: got_to_xy
Launch the turtlesim_node then launch go_to_x. This simply subscribes to the turtles location, then issues cmd_vel messages to move the turtle to the goal designated as a constant on line 16. 

Subscribed Topics:
/turtle1/pose ([turtlesim::PoseConstPtr])
The turtle's pose

/waypoint ([geometry_msgs::Pose2D])
The desired location



Published Topics:

turtle1/cmd_vel ([geometry_msgs::Twist])
Publishes commands to move the turtle to the desired x, y coordinates




Node: got_to_x

Subscribed Topics:

none


Published Topics:

/waypoint ([geometry_msgs::Pose2D])
The desired location entered by the user


