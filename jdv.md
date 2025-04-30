# JaiaBot Data Vision

The JaiaBot Data Vision system is a web server that allows client browsers to plot data graphs and maps, generated from .goby / .h5 files that are stored on the server.

##  Launching the JDV web interface
```
cd /path/to/jaiabot/src/web/jdv
./run.sh
# Then in browser enter link 
http://172.22.203.139:40011
```

# JDV Interface: Button Functions Explained
<table>
  <tr>
    <th>Button</th>
    <th>Image</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>System Check All Bots</td>
    <td><img src="https://raw.githubusercontent.com/Kait211/Practice/main/Add%20Plot.png" alt="System Check All Bots" style="width: 100px; height: auto;"></td>
    <td>Run a system check on all bots in the pod. Missions can only be run after the system check completes successfully.</td>
  </tr>
</table>


# Jaiabot software
For instructions for how to running JDV with the bot_offload log directory refer to https://github.com/jaiarobotics/jaiabot/blob/1.y/src/doc/markdown/page120_working_with_jaia_software.md

## Overview

The Jaiabot Data Vision is directly launched using a script (run.sh) that starts both the Flask API and the React frontend server

### JDV Web App
The run.sh script launches a Flask application which implements a REST API for getting log data and data series from the `goby` and `.h5` files in the `~/jaia-logs/bot_offload` directory. It also serves a browser-based client application built with React. The frontend is automatically built and placed in the `~/jaiabot/build/web_dev/jdv` when running run.sh. No manual React build step is needed.
