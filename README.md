# PowerShell Heuristic-Confuser

This PowerShell script attempts to bypass AV heuristic or sandbox detection by date/time comparisons.  

Heuristic AV or sandbox detections will often ignore long sleeps when running payloads in a sandbox for analysis. This is done mostly as to not to inconvenience the user too much. 

We can take advantage of this by taking the date before and after a long sleep to see if they match up. If not the script will simply exit not producing any detectable actions or IoCs. For example, in a sandbox, if time magically fast-forwarded, thus skipping the sleep. 

Just place your (obfuscated) script or command into the "Else" statement. Enjoy!

Use at your own risk! For educational purposes only.

