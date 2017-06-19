#include "ros/ros.h"
#include "std_msgs/String.h"
#include "geometry_msgs/Twist.h"
#include "geometry_msgs/PolygonStamped.h"
#include <dynamic_reconfigure/DoubleParameter.h>
#include <dynamic_reconfigure/Reconfigure.h>
#include <dynamic_reconfigure/Config.h>

/*
dynamic_reconfigure::ReconfigureRequest srv_req;
dynamic_reconfigure::ReconfigureResponse srv_resp;
dynamic_reconfigure::geometry_msgs::PolygonStamped double_param;
dynamic_reconfigure::Config conf;*/

//ros::Publisher footprint_pub;

void VelocityCallback(const geometry_msgs::Twist::ConstPtr& msg)
{
  ROS_INFO("x: [%f]", msg->linear.x);
  ROS_INFO("o: [%f]", msg->angular.y);

  double vel = msg->linear.x;

  if ((vel > -66.6) && (vel <= 0)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-0.38,-0.32],[-0.38,0.32], [0.38, 0.32], [0.38,-0.32]]'");
	system("rosrun dynamic_reconfigure dynparam set /move_base/local_costmap footprint '[[-0.38,-0.32],[-0.38,0.32], [0.38, 0.32], [0.38,-0.32]]'");

	//std_msgs::String msg_footprint;
	//geometry_msgs::PolygonStamped msg_footprint;
	//msg_footprint.header.seq = msg->header.seq;
	//msg_footprint.header.stamp = msg->header.stamp;
	//msg_footprint.header.frame_id = msg->header.frame_id;
/*
	msg_footprint.polygon.points[0].x = msg_footprint.polygon.points[0].x + 1;
	msg_footprint.polygon.points[0].y = msg_footprint.polygon.points[0].y + 1;

	msg_footprint.polygon.points[1].x = msg_footprint.polygon.points[1].x + 1;
	msg_footprint.polygon.points[1].y = msg_footprint.polygon.points[1].y + 1;

	msg_footprint.polygon.points[2].x = msg_footprint.polygon.points[2].x + 1;
	msg_footprint.polygon.points[2].y = msg_footprint.polygon.points[2].y + 1;

	msg_footprint.polygon.points[3].x = msg_footprint.polygon.points[3].x + 1;
	msg_footprint.polygon.points[3].y = msg_footprint.polygon.points[3].y + 1;

	//msg_footprint.data = "[[-1,-1],[-1,1], [1, 1], [1,-1]]";
	footprint_pub.publish(msg_footprint);*/
  
  } else if ((vel > 0) && (vel <= 0.27)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-0.55,-0.46],[-0.55,0.46], [0.55, 0.46], [0.55,-0.46]]'");
	system("rosrun dynamic_reconfigure dynparam set /move_base/local_costmap footprint '[[-0.55,-0.46],[-0.55,0.46], [0.55, 0.46], [0.55,-0.46]]'");
  /*
    double_param.name = "local_costmap/footprint";
    double_param.value = "[[-0.45,-0.36],[-0.45,0.36], [0.45, 0.36], [0.45,-0.36]]";
    conf.doubles.push_back(double_param);

    double_param.name = "global_costmap/footprint";
    double_param.value = "[[-0.45,-0.36],[-0.45,0.36], [0.45, 0.36], [0.45,-0.36]]";
    conf.doubles.push_back(double_param);

    srv_req.config = conf;

    ros::service::call("/move_base", srv_req, srv_resp);*/
  
  } else if ((vel > 0.27) && (vel <= 0.57)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-0.65,-0.56],[-0.65,0.56], [0.65, 0.56], [0.65,-0.56]]'");
	system("rosrun dynamic_reconfigure dynparam set /move_base/local_costmap footprint '[[-0.65,-0.56],[-0.65,0.56], [0.65, 0.56], [0.65,-0.56]]'");

  } else if ((vel > 0.57) && (vel <= 0.67)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-0.75,-0.66],[-0.75,0.66], [0.75, 0.66], [0.75,-0.66]]'");
	system("rosrun dynamic_reconfigure dynparam set /move_base/local_costmap footprint '[[-0.75,-0.66],[-0.75,0.66], [0.75, 0.66], [0.75,-0.66]]'");	

  } else if ((vel > 0.67) && (vel <= 0.77)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-0.85,-0.76],[-0.85,0.76], [0.85, 0.76], [0.85,-0.76]]'");
	system("rosrun dynamic_reconfigure dynparam set /move_base/local_costmap footprint '[[-0.85,-0.76],[-0.85,0.76], [0.85, 0.76], [0.85,-0.76]]'");

  } else if ((vel > 0.77) && (vel <= 0.97)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-0.95,-0.86],[-0.95,0.86], [0.95, 0.86], [0.95,-0.86]]'");
  
  } else if ((vel > 0.97) && (vel <= 1.17)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-1.05,-0.96],[-1.05,0.96], [1.05, 0.96], [1.05,-0.96]]'");
  
  } else if ((vel > 1.17) && (vel <= 1.27)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-1.15,-1.06],[-1.15,1.06], [1.15, 1.06], [1.15,-1.06]]'");
  
  } else if ((vel > 1.27) && (vel <= 1.37)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-1.25,-1.16],[-1.25,1.16], [1.25, 1.16], [1.25,-1.16]]'");
  
  } else if ((vel > 1.37) && (vel <= 1.47)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-1.35,-1.26],[-1.35,1.26], [1.35, 1.26], [1.35,-1.26]]'");
  
  } else if ((vel > 1.47) && (vel <= 1.57)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-1.45,-1.36],[-1.45,1.36], [1.45, 1.36], [1.45,-1.36]]'");
  
  } else if ((vel > 1.57) && (vel <= 66.6)){

	system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-1.55,-1.46],[-1.55,1.46], [1.55, 1.46], [1.55,-1.46]]'"); 
  }
}

int main(int argc, char **argv)
{

  ros::init(argc, argv, "dynamic_footprint");

  ros::NodeHandle n;

  system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-0.38,-0.32],[-0.38,0.32], [0.38, 0.32], [0.38,-0.32]]'");
  system("rosrun dynamic_reconfigure dynparam set /move_base/local_costmap footprint '[[-0.38,-0.32],[-0.38,0.32], [0.38, 0.32], [0.38,-0.32]]'");

  //n.setParam("/move_base/global_costmap/footprint", "[[-1,-1],[-1,1],[1,1],[1,-1]]");
 
  //ros::Publisher footprint_pub = n.advertise<std_msgs::String>("move_base/global_costmap/footprint", 1000);
  ros::Subscriber sub = n.subscribe("yocs_cmd_vel_mux/cmd_vel", 1000, VelocityCallback);

  //system("rosrun dynamic_reconfigure dynparam set /move_base/global_costmap footprint '[[-1,-1],[-1,1], [1, 1], [1,-1]]'");

  ros::spin();

  return 0;
}
