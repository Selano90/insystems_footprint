#! /usr/bin/env python
import rospy
import roslib
import dynamic_reconfigure.client
from geometry_msgs.msg import Twist

states=[0,0,0,0,0,0,0,0]
def callback(data):
    global client,client_2,states
    x=data.linear.x
       
    if (x>-66.6) and (x<=0) and states[0]==0 :
	rospy.loginfo("x = %f", x)
        params = { 'footprint' : '[[0.34,0.34], [-0.34,0.34], [-0.4,0.3], [-0.4,-0.3], [-0.34,-0.34], [0.34,-0.34], [0.4,-0.28], [0.4,0.28]]'  }
        config = client.update_configuration(params)
	params_2 = { 'footprint' : '[[0.34,0.34], [-0.34,0.34], [-0.4,0.3], [-0.4,-0.3], [-0.34,-0.34], [0.34,-0.34], [0.4,-0.28], [0.4,0.28]]'  }
        config_2 = client_2.update_configuration(params_2)	
        for i in range(0,6):
            if (i ==0):
                states[i]+=1
	    else:
		states[i]=0       
    elif (x > 0) and (x <= 0.27) and states[1]==0 :
	rospy.loginfo("x = %f", x)
        params = { 'footprint' : '[[0.39,0.39], [-0.39,0.39], [-0.45,0.35], [-0.45,-0.35], [-0.39,-0.39], [0.39,-0.39], [0.45,-0.33], [0.45,0.33]]'  }
        config = client.update_configuration(params)
	params_2 = { 'footprint' : '[[0.39,0.39], [-0.39,0.39], [-0.45,0.35], [-0.45,-0.35], [-0.39,-0.39], [0.39,-0.39], [0.45,-0.33], [0.45,0.33]]'  }
        config_2 = client_2.update_configuration(params_2)
	for i in range(0,6):
            if (i ==1):
                states[i]+=1
	    else:
		states[i]=0 
    elif (x > 0.27) and (x <= 0.57) and states[2]==0:
	rospy.loginfo("x = %f", x)
        params = { 'footprint' : '[[0.44,0.44], [-0.44,0.44], [-0.5,0.4], [-0.5,-0.4], [-0.44,-0.44], [0.44,-0.44], [0.5,-0.38], [0.5,0.38]]' }
        config = client.update_configuration(params)
	params_2 = { 'footprint' : '[[0.44,0.44], [-0.44,0.44], [-0.5,0.4], [-0.5,-0.4], [-0.44,-0.44], [0.44,-0.44], [0.5,-0.38], [0.5,0.38]]' }
        config_2 = client_2.update_configuration(params_2)
	for i in range(0,6):
            if (i ==2):
                states[i]+=1
	    else:
		states[i]=0 
    elif (x > 0.57) and (x <= 0.67) and states[3]==0:
	rospy.loginfo("x = %f", x)
        params = { 'footprint' : '[[0.49,0.49], [-0.49,0.49], [-0.55,0.45], [-0.55,-0.45], [-0.49,-0.49], [0.49,-0.49], [0.55,-0.43], [0.55,0.43]]'  }
        config = client.update_configuration(params)
	params_2 = { 'footprint' : '[[0.49,0.49], [-0.49,0.49], [-0.55,0.45], [-0.55,-0.45], [-0.49,-0.49], [0.49,-0.49], [0.55,-0.43], [0.55,0.43]]'  }
        config_2 = client_2.update_configuration(params_2)
	for i in range(0,6):
            if (i ==3):
                states[i]+=1
	    else:
		states[i]=0 
    elif (x > 0.67) and (x <= 0.77) and states[4]==0:
	rospy.loginfo("x = %f", x)
        params = { 'footprint' : '[[0.54,0.54], [-0.54,0.54], [-0.6,0.5], [-0.6,-0.5], [-0.54,-0.54], [0.54,-0.54], [0.6,-0.48], [0.6,0.48]]' }
        config = client.update_configuration(params)
	params_2 = { 'footprint' : '[[0.54,0.54], [-0.54,0.54], [-0.6,0.5], [-0.6,-0.5], [-0.54,-0.54], [0.54,-0.54], [0.6,-0.48], [0.6,0.48]]' }
        config_2 = client_2.update_configuration(params_2)
	for i in range(0,6):
            if (i ==4):
                states[i]+=1
	    else:
		states[i]=0 
    elif (x > 0.77) and (x <= 0.87) and states[5]==0:
	rospy.loginfo("x = %f", x)
        params = { 'footprint' : '[[0.59,0.59], [-0.59,0.59], [-0.65,0.55], [-0.65,-0.55], [-0.59,-0.59], [0.59,-0.59], [0.65,-0.53], [0.65,0.53]]' }
        config = client.update_configuration(params)
	params_2 = { 'footprint' : '[[0.59,0.59], [-0.59,0.59], [-0.65,0.55], [-0.65,-0.55], [-0.59,-0.59], [0.59,-0.59], [0.65,-0.53], [0.65,0.53]]'}
        config_2 = client_2.update_configuration(params_2)
	for i in range(0,6):
            if (i ==5):
                states[i]+=1
	    else:
		states[i]=0 
    elif (x > 0.87) and (x <= 0.97) and states[5]==0:
        rospy.loginfo("x = %f", x)
        params = { 'footprint' : '[[0.64,0.64], [-0.64,0.64], [-0.7,0.6], [-0.7,-0.6], [-0.64,-0.64], [0.64,-0.64], [0.7,-0.58], [0.7,0.58]]' }
        config = client.update_configuration(params)
        params_2 = { 'footprint' : '[[0.64,0.64], [-0.64,0.64], [-0.7,0.6], [-0.7,-0.6], [-0.64,-0.64], [0.64,-0.64], [0.7,-0.58], [0.7,0.58]]'}
        config_2 = client_2.update_configuration(params_2)
        for i in range(0,6):
            if (i ==6):
                states[i]+=1
            else:
                states[i]=0
    elif (x > 0.97) and (x <= 1.07) and states[5]==0:
        rospy.loginfo("x = %f", x)
        params = { 'footprint' : '[[0.69,0.69], [-0.69,0.69], [-0.75,0.65], [-0.75,-0.65], [-0.69,-0.69], [0.69,-0.69], [0.75,-0.63], [0.75,0.63]]'  }
        config = client.update_configuration(params)
        params_2 = { 'footprint' : '[[0.69,0.69], [-0.69,0.69], [-0.75,0.65], [-0.75,-0.65], [-0.69,-0.69], [0.69,-0.69], [0.75,-0.63], [0.75,0.63]]'  }
        config_2 = client_2.update_configuration(params_2)
        for i in range(0,6):
            if (i ==7):
                states[i]+=1
            else:
                states[i]=0

def main():
    global client, client_2
    rospy.init_node('dynamit', anonymous=True)
    rospy.Subscriber("/yocs_cmd_vel_mux/cmd_vel", Twist, callback)
    rate=rospy.Rate(10)
    done=False
    while not done:
        try :

            client = dynamic_reconfigure.client.Client("/move_base/global_costmap", timeout=1)
            params = { 'footprint' : '[[0.34,0.34], [-0.34,0.34], [-0.4,0.3], [-0.4,-0.3], [-0.34,-0.34], [0.34,-0.34], [0.4,-0.28], [0.4,0.28]]' }
            config = client.update_configuration(params)
            client_2 = dynamic_reconfigure.client.Client("/move_base/local_costmap", timeout=1)
            params_2 = { 'footprint' : '[[0.34,0.34], [-0.34,0.34], [-0.4,0.3], [-0.4,-0.3], [-0.34,-0.34], [0.34,-0.34], [0.4,-0.28], [0.4,0.28]]' }
            config_2 = client_2.update_configuration(params_2)
            done=True
        except rospy.exceptions.ROSException :
            pass 
        rate.sleep()
    rospy.spin()
if __name__ == '__main__':
    try :
        main()
    except rospy.exceptions.ROSException :
        pass
