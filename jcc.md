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
    <td valign="top">Stop All Missions</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20All%20Missions.png" alt="Stop ALL Missions" style="width: 50px; height: 40px;"></td>
    <td valign="top">Order all bots to stop their currently running missions.</td>
  </tr>
   <tr>
    <td valign="top">Run All Missions</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Run%20All%20Missions.png" alt="Run All Missions" style="width: 50px; height: 40px;"></td>
    <td valign="top">Run the mission as currently edited on the map.</td>
  </tr>
  <tr>
    <td valign="top">Download All</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Download%20All.png" alt="Download All" style="width: 50px; height: 40px;"></td>
    <td valign="top">Start downloading log and sensor data from all of the bots to the hub.</td>
  </tr>
  <tr>
    <td valign="top">Undo</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Undo.png" alt="Undo" style="width: 50px; height: 40px;"></td>
    <td valign="top">Undo the last 10 mission planning actions (excluding Task modifications).</td>
  </tr>
  <tr>
    <td valign="top">Mission Panel</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Mission%20Panel.png" alt="Mission Panel" style="width: 50px; height: 40px;"></td>
    <td valign="top">Open the Mission Panel, which shows each run in the current mission, along with the bots assigned to each run. Bots can be auto-assigned to runs automatically. Missions can also be saved, loaded, and cleared from this panel.</td>
  </tr>
  <tr>
    <td valign="top">Add Rally Point</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Add%20Rally%20Point.png" alt="Add Rally Point" style="width: 50px; height: 40px;"></td>
    <td valign="top">Add a rally point that can be used at the start or end of a survey mission.</td>
  </tr>
  <tr>
    <td valign="top">Edit Optimized Mission Survey</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Edit%20Optimized%20Mission%20Survey.png" alt="Edit Optimized Mission Survey" style="width: 50px; height: 40px;"></td>
    <td valign="top">Open the Optimized Mission Survey, which can be used to configure a survey mission, where the pod of Jaiabots will coordinate to survey an area of the map. The tasks performed at each waypoint in the survey mission can be customized.</td>
  </tr>
  <tr>
    <td valign="top">Download Queue</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Download%20Queue.png" alt="Download Queue" style="width: 50px; height: 40px;"></td>
    <td valign="top">Open the Download Queue panel, which shows the currently queued data downloads from the bots to the hub.</td>
  </tr>
  <tr>
    <td valign="top">Measure Distance</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Measure%20Distance.png" alt="Measure Distance" style="width: 50px; height: 40px;"></td>
    <td valign="top">Click two or more points to measure the total distance along a set of line segment</td>
  </tr>
  <tr>
    <td valign="top">Settings</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Settings.png" alt="Settings" style="width: 50px; height: 40px;"></td>
    <td valign="top">Open the Settings panel for Jaia Command & Contro</td>
  </tr>
  <tr>
    <td valign="top">Reset rotation</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Reset%20Rotation.png" alt="Reset rotation" style="width: 50px; height: 40px;"></td>
    <td valign="top">When using tablet, click to reset rotation of the map.</td>
  </tr>
  <tr>
    <td valign="top">Zoom in</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Zoom%20In.png" alt="Zoom in" style="width: 50px; height: 40px;"></td>
    <td valign="top">Increase the map's magnification.</td>
  </tr>
  <tr>
    <td valign="top">Zoom out</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Zoom%20Out.png" alt="Zoom out" style="width: 50px; height: 40px;"></td>
    <td valign="top">Decrease the map's magnification.</td>
  </tr>
  </table>

  # Hub Commands
  <table>
  <tr>
    <th>Button Name</th>
    <th>Image</th>
    <th>Description</th>
  </tr>
  <tr>
    <td valign="top">Shutdown</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Shutdown.png" alt="ShutDown" style="width: 50px; height: 40px;"></td>
    <td valign="top">Shutdowns the system for the Hub.</td>
  </tr>
  <tr>
    <td valign="top">Reboot</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Reboot.png" alt="Reboot" style="width: 50px; height: 40px;"></td>
    <td valign="top">Reboots the Hub.</td>
  </tr>
  <tr>
    <td valign="top">Restart</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Restart.png" alt="Restart" style="width: 50px; height: 40px;"></td>
    <td valign="top">Restart the Hub.</td>
  </tr>
  <tr>
    <td valign="top">JDV</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/JDV.png" alt="JDV" style="width: 50px; height: 40px;"></td>
    <td valign="top">Link for Jaia Data Vision (JDV).</td>
  </tr>
  <tr>
    <td valign="top">JED</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/JED.png" alt="JED" style="width: 50px; height: 40px;"></td>
    <td valign="top">Link for Jaia Engineering and Debugging (JED)</td>
  </tr>
  <tr>
    <td valign="top">Router</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Router.png" alt="Router" style="width: 50px; height: 40px;"></td>
    <td valign="top">Link for router.</td>
  </tr>
  <tr>
    <td valign="top">Upgrade</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Upgrade.png" alt="Upgrade" style="width: 50px; height: 40px;"></td>
    <td valign="top">Link for upgrades.</td>
  </tr>
</table>

# Bot Commands
<table>
  <tr>
    <th>Button Name</th>
    <th>Image</th>
    <th>Description</th>
  </tr>
  <tr>
    <td valign="top">Stop Mission</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Stop%20Mission.png" alt="Stop Mission" style="width: 50px; height: 40px;"></td>
    <td valign="top">Stop mission for a chosen bot.</td>
  </tr>
  <tr>
    <td valign="top">Run Mission</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Run%20All%20Missions.png" alt="Run Mission" style="width: 50px; height: 40px;"></td>
    <td valign="top">Play mission for a chosen bot.</td>
  </tr>
   <tr>
    <td valign="top">Clear Mission</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/Clear%20Mission.png" alt="Run Mission" style="width: 50px; height: 40px;"></td>
    <td valign="top">Clear mission for a chosen bot.</td>
  </tr>
  <tr>
    <td valign="top">RC mode</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jcc/RC%20mode.png" alt="RC mode" style="width: 50px; height: 40px;"></td>
    <td valign="top">	Romote controller to control Manual Dual, Manual Single, and Dive. User can use throttle to move forward/backwards and rudder to change direction.</td>
  </tr>