## View the robot with rviz

For every change you make in the URDFs inside src/pisa/description for some reason you have to run

```bash
colcon build --symlink-install
source install/setup.zsh
```

Then, run the launch publisher:

```bash
ros2 launch pisa rsp.launch.py
ros2 run joint_state_publisher_gui joint_state_publisher_gui
 ```

Right! now you're publishing the urdfs in a ros topic, to view it just run rviz

```bash
rviz2 -d src/pisa/config/view_bot.rviz 
 ```
