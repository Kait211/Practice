# JaiaBot Data Vision

The JaiaBot Data Vision system is a web server that allows client browsers to plot data graphs and maps, generated from .goby / .h5 files that are stored on the server.

## Launching the JDV web interface

```
cd /path/to/jaiabot/src/web/jdv
./run.sh
# Then in browser enter link
http://172.22.203.139:40011
```

# JDV Interface: 
### Plot Controls Explained

<table>
  <tr>
    <th>Button Name</th>
    <th>Image</th>
    <th>Description</th>
  </tr>
  <tr>
    <td valign="top">Add Plot</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jdv/client/src/images/Add%20Plot.png" alt="Add Plot" style="width: 50px; height: 40px;"></td>
    <td valign="top">Add plots to the map to visualize bot data</td>
  </tr>
  <tr>
    <td valign="top">Load Plot Set</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jdv/client/src/images/Load%20Plot%20Set.png" alt="Load Plot Set" style="width: 50px; height: 40px;"></td>
    <td valign="top">Load a saved plot set to visualize bot data on the map</td>
  </tr>
  <tr>
    <td valign="top">Save Plot Set</td>
    <td valign="top"><img src= "https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jdv/client/src/images/Save%20Plot%20Set.png"
     alt="Save Plot Set" style="width: 50px; height: 40px;"></td>
    <td valign="top">Save the current plot set for later retrieval</td>
  </tr>
  <tr>
    <td valign="top">Download CSV</td>
    <td valign="top"><img src= "https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jdv/client/src/images/Download%20CSV.png"
     alt="Download CSV" style="width: 50px; height: auto;"></td>
    <td valign="top">Download plot set data into a CSV file</td>
  </tr>
  <tr>
    <td valign="top">Clear Plots</td>
    <td valign="top"><img src= "https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jdv/client/src/images/Clear%20Plots.png"
     alt="Clear Plots" style="width: 50px; height: auto;"></td>
    <td valign="top">Clear all plots from the JDV interface</td>
  </tr>
</table>

### Map Controls Explained
<table>
  <tr>
    <th>Button Name</th>
    <th>Image</th>
    <th>Description</th>
  </tr>
  <tr>
    <td valign="top">Layer Switch Toggler</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jdv/client/src/images/Layer%20Switch%20Toggler.png" alt="Layer Switch Toggler" alt="Layer Switch Toggler" style="width: 50px; height: auto;"></td>
    <td valign="top">Switch between Base map and different layers of data displayed on the map</td>
  </tr>
  <tr>
    <td valign="top">KML Export</td>
    <td valign="top"><img src="https://raw.githubusercontent.com/jaiarobotics/jaiabot/task/update-environment-setup-documentation/src/web/jdv/client/src/images/KML%20Export%20Button.png" alt="Layer Switch Toggler" alt="KML Export" style="width: 50px; height: auto;"></td>
    <td valign="top">Export the plotted data as a KML file for use in mapping applications</td>
  </tr>
  </table>

# Jaiabot software

For instructions for how to running JDV with the bot_offload log directory refer to https://github.com/jaiarobotics/jaiabot/blob/1.y/src/doc/markdown/page120_working_with_jaia_software.md

## Overview

The Jaiabot Data Vision is directly launched using a script (run.sh) that starts both the Flask API and the React frontend server

### JDV Web App

The run.sh script launches a Flask application which implements a REST API for getting log data and data series from the `goby` and `.h5` files in the `~/jaia-logs/bot_offload` directory. It also serves a browser-based client application built with React. The frontend is automatically built and placed in the `~/jaiabot/build/web_dev/jdv` when running run.sh. No manual React build step is needed.
