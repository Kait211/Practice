# Jaia Command and Control

Jaia Command and Control (JCC) is a mission planning and control application for managing JaiaBots and JaiaHubs. It allows users to create, configure, and execute missions, monitor the health status of the bots, and download mission data from the bots.

# Launcing JCC interface

Note: These steps assume the simulator has already been built. For instructions on building the simulator, refer to https://github.com/jaiarobotics/jaiabot/blob/1.y/src/doc/markdown/page120_working_with_jaia_software.md

1. Launch the JCC web interface

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

3. In browser enter URL
```
http://localhost:40001
```

# JCC Button Commands

<table>
  <tr>
    <th>Button Name</th>
    <th>Image</th>
    <th>Description</th>
  </tr>
  <tr>
    <td valign="top">System Check All Bots</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/System_Check_All_Bots.png" alt="System Check All Bots" style="width: 50px; height: 40px;"></td>
    <td valign="top">Run a system check on all bots in the pod. Missions can only be run after the system check completes successfully.</td>
  </tr>
    <tr>
    <td valign="top">Stop ALL Missions</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Undo.png" alt="Stop ALL Missions" style="width: 50px; height: 40px;"></td>
    <td valign="top">Order all bots to stop their currently running missions.</td>
  </tr>
  <tr>
    <td valign="top">Mission Panel</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Mission Panel" style="width: 50px; height: 40px;"></td>
    <td valign="top">Open the Mission Panel, which shows each run in the current mission, along with the bots assigned to each run. Bots can be auto-assigned to runs automatically. Missions can also be saved, loaded, and cleared from this panel.</td>
  </tr>
  <tr>
    <td valign="top">Add Rally Point</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Add Rally Point" style="width: 50px; height: 40px;"></td>
    <td valign="top">Add a rally point that can be used at the start or end of a survey mission.</td>
  </tr>
  <tr>
    <td valign="top">Edit Optimized Mission Survey</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Edit Optimized Mission Survey" style="width: 50px; height: 40px;"></td>
    <td valign="top">Open the Optimized Mission Survey, which can be used to configure a survey mission, where the pod of Jaiabots will coordinate to survey an area of the map. The tasks performed at each waypoint in the survey mission can be customized.</td>
  </tr>
  <tr>
    <td valign="top">Download Queue</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Download Queue" style="width: 50px; height: 40px;"></td>
    <td valign="top">Open the Download Queue panel, which shows the currently queued data downloads from the bots to the hub.</td>
  </tr>
  <tr>
    <td valign="top">Measure Distance</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Measure Distance" style="width: 50px; height: 40px;"></td>
    <td valign="top">Click two or more points to measure the total distance along a set of line segment</td>
  </tr>
  <tr>
    <td valign="top">Settings</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Settings" style="width: 50px; height: 40px;"></td>
    <td valign="top">Open the Settings panel for Jaia Command & Contro</td>
  </tr>
  <tr>
    <td valign="top">Reset rotation</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Reset rotation" style="width: 50px; height: 40px;"></td>
    <td valign="top">When using tablet, click to reset rotation of the map.</td>
  </tr>
  <tr>
    <td valign="top">Zoom in</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Zoom in" style="width: 50px; height: 40px;"></td>
    <td valign="top">Increase the map's magnification.</td>
  </tr>
  <tr>
    <td valign="top">Zoom out</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Zoom out" style="width: 50px; height: 40px;"></td>
    <td valign="top">Decrease the map's magnification.</td>
  </tr>
