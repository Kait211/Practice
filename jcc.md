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