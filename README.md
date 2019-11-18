# ur_extra_changes
Those are the extra changes needed so that the driver or the arm + wrist cam + gripper would work

## Changes:

- universal_robot/ur5_e_moveit_config/config/controllers.yaml: change name "" to "scaled_pos_traj_controller"

## Files added:

- Universal_Robots_ROS_Driver/ur_robot_driver/launch/ur5e_cam_2f85_bringup.launch

- universal_robot/ur_e_description/launch/ur5e_cam_2f85_upload.launch

- universal_robot/ur_e_description/launch/view_ur5e_cam_2f85.launch

- universal_robot/ur_e_description/urdf/ur5e_cam_2f85_robot.urdf.xacro

- universal_robot/ur_e_description/urdf/ur5e_cam_2f85_joint_limited_robot.urdf

- robotiq/robotiq_2f_85_gripper_visualization/urdf/robotiq_cam.xacro

## Directory added:

- universal_robot/ur5e_cam_2f85_moveit_config

## Directary: other

If the arm + gripper moveit config directary needs to be re-generated, the launch files in the the other directory will need to be replaced so that the "limited" UR planner could work.