### Test Cases And Observations Table
<table>
  <tr>
    <th>Test Case</th>
    <th>Expected Outcome</th>
    <th>Actual Outcome</th>
    <th>Issues/Errors</th>
    <th>Notes</th>
  </tr>
  <tr>
    <td valign="top">Hover over all icons to check labels.</td>
    <td valign="top">Each icon displays a label.</td>
    <td valign="top">Each icon has labels, and the “Help” icon explains their functions except for “Reset Rotation,” “Zoom In,” and “Zoom Out.”</td>
    <td valign="top">No issues or errors.</td>
    <td valign="top">The labels for icons on the right of the interface are:  
      <ul>
        <li><strong>System Check All Bots</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/System_Check_All_Bots.png" alt="System Check" />
        </li>
        <li><strong>Stop All Missions</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Stop%20All%20Missions.png" alt="Stop All Missions" />
        </li>
        <li><strong>Run All Missions</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Run%20All%20Missions.png" alt="Run All Missions" />
        </li>
        <li><strong>Download All</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Download%20All.png" alt="Download All" />
        </li>
        <li><strong>Undo</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Undo.png" alt="Undo" />
        </li>
        <li><strong>Help</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Help.png" alt="Help" />
        </li>
        <li><strong>Mission Panel</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Mission%20Panel.png" alt="Mission Panel" />
        </li>
        <li><strong>Add Rally Point</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Add%20Rally%20Point.png" alt="Add Rally Point" />
        </li>
        <li><strong>Edit Optimized Mission Survey</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Edit%20Optimized%20Mission%20Survey.png" alt="Edit Optimized Mission Survey" />
        </li>
        <li><strong>Download Queue</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Download%20Queue.png" alt="Download Queue" />
        </li>
        <li><strong>Measure Distance</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Measure%20Distance.png" alt="Measure Distance" />
        </li>
        <li><strong>Settings</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Settings.png" alt="Settings" />
        </li>
        <li><strong>Reset Rotation</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Reset%20Rotation.png" alt="Reset Rotation" />
        </li>
        <li><strong>Zoom In</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Zoom%20In.png" alt="Zoom In" />
        </li>
        <li><strong>Zoom Out</strong><br> 
          <img src="https://raw.githubusercontent.com/Kait211/Practice/main/Zoom%20Out.png" alt="Zoom Out" />
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td valign="top">Place waypoints and “Run Mission” with a bot.</td>
    <td valign="top">The Bot should “Run Mission” and show run through the waypoints.</td>
    <td valign="top">The bot went to the end waypoint, but I did not see the journey.</td>
    <td valign="top">No issues/errors.</td>
    <td valign="top">I would put an animation to see the journey the bot takes from beginning to end.
</td>
  </tr>
  <tr>
    <td valign="top">"Run Mission" with waypoints, then edit the waypoints to add new ones and "Run Mission" again.</td>
    <td valign="top">The bot should travel the edited waypoint route when I hit "Run Mission" on the bot.</td>
    <td valign="top">The bot navigated the initial waypoints successfully, but after editing the route and pressing "Run Mission," it remained at waypoint 4 instead of proceeding to waypoint 8.</td>
    <td valign="top">Possible issue here: the bot should travel to waypoint 8 after the route was edited and the mission was set to run.</td>
    <td valign="top">I wonder if users are supposed to do it another way to make the bot travel the edited route, or if once the mission starts, you can’t make the bot change positions later.
</td>
  </tr>
  <tr>
    <td valign="top">Run "System Check On All Bots".</td>
    <td valign="top">System check completes without errors.</td>
    <td valign="top">The sim displays the message, "Click the OK button to activate Bots: 1, 2, 3, 4." The system check was successful for all bots.</td>
    <td valign="top">No issues or errors.</td>
    <td valign="top">Missions cannot start unless the "System Check On All Bots" is completed.
</td>
  </tr>
  <tr>
    <td valign="top">Run system check with offline bots.</td>
    <td valign="top">Offline bots are flagged, and system check fails.</td>
    <td valign="top">When I clicked run systems, it says "Alert: The command cannot be sent to Bots: 1, 2, 3, 4 because the status age is greater than 30."</td>
    <td valign="top">No issues or errors</td>
    <td valign="top">What does status age mean? Time bot has been unconnected to the hub possibly?
</td>
  </tr>
</table>
