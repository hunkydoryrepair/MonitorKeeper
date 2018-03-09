# MonitorKeeper
Return windows to their rightful place when changing monitors. 

Author: Garr Godfrey<br>
License: MIT License<br>
License Summary: Free but author takes no responsibility.<br>
//<br>
<p>
Monitor Keeper is a simple app that runs as an application on the task bar that will restore windows
to their original locations when a monitor because available. When a monitor is turned off, or HDMI is unplugged,
Windows 7 and higher detect that and will rearrange all application windows onto the remaining monitor(s).
If the monitor is reconnected, the applications stay on the single monitor, requiring the user to
move them back manually. This application moves them back automatically.
</p>
//<br>
Limitations:<br>
<ul>
		<li> Windows are only repositions when the number of monitors INCREASES. There is no way to specify a layout
			to use on a single monitor, for example (although this would not be a difficult change)</li>
		<li> Support is limited to 5 monitors. This is arbitrary and done simply to limit the storage for each application.</li>
		<li> If application is run as a standard user, it cannot move any applications that are running as a privileged user.
			If you run into this, you can run this program as administrator, perhaps using Task Scheduler to launch it at login.</li>
		<li> Window position is only saved while application is running. There is no persistent storage of position (say, between reboots)</li>
		<li> Windows will return to their state when the number of monitors was most recently seen. So, a window may go from minimize to
			maximized or be a different size once the second (or third) monitor is plugged back in.</li>
</ul>
//
DEMO:<br>
<p>
		To quickly test the functionality, go to Display Settings... in windows (right click on desktop), with two monitors, change
 the setting for "Multiple Displays" from "Extend These Displays" to "Duplicate These Displays".  Compare when running Monitor
 Keeper and when not.
 </p>
