# Jaiabot Engineer and Debug

The JaiaBot Engineer & Debug is a utility application that allows engineers and developers to send low-level engineering commands directly to JaiaBots. Users can use this application to adjust motor and rudder values, initiate IMU calibration, perform echo testing, and conduct dives with specified throttle and rudder settings. The application receives data in real time and can be used for debugging purposes.

# Accessing the JED interface

1. Launch the JCC web interface
   Note: If needed steps for setting up the simulator to launch JCC interface, are located in the markdown file https://github.com/jaiarobotics/jaiabot/blob/1.y/src/doc/markdown/page120_working_with_jaia_software.md

```
cd /path/to/jaiabot/src/web
./run.sh
```

2. Launch the simulator in a separate terminal

```
cd /path/to/jaiabot/config/launch/simulation
# Set the simulation to run 4 bots at a time warp of 5
./generate_all_launch.sh 4 5
./all.launch
```

3. In browser enter link

```
http://localhost:40001
```

4. Click on Hub button

![HUB Button](https://github.com/jaiarobotics/jaiabot/blob/task/update-environment-setup-documentation/src/web/jed/HUB_Button.png?raw=true)

5. Click on JED button

![JED Button](https://github.com/jaiarobotics/jaiabot/blob/task/update-environment-setup-documentation/src/web/jed/JED_Button.png?raw=true)

