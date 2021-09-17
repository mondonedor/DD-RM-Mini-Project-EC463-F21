Report

Once the Raspberry Pi was set up, the wifi_scan.py script was run for approximately fifteen minutes. The location that the Pi was set up in was an apartment near a street intersection. Measuring the amount of wi-fi hotspots detected over the scanning duration could give an estimate of the amount of vehicles that passed through the intersection over that time.

The json data file produced by the wifi_scan.py script was then passed into the wifi_plot script to produce the plot found attached to this repository. The horizontal axis shows the time interval that the scans were conducted on and the vertical axis shows the amount of wi-fi hotspots detected from scans in a continuous fashion. Something to note is that the wi-fi scans sometimes did not actually pick up an ESSID. The provided wifi_plot.py script was modified with an error catch line to handle these cases.

Over the scanning duration, anywhere between about four and nineteen hotspots were detected. One can clearly see numerous oscillations with the amount of wi-fi hotspots detected every few minutes, which shows that vehicles transiting the nearby intersection possibly appear in many separate waves rather than in a more continuous, consistent level of traffic.

Looking at the raw json file data, one can also see that many other stationary devices were detected in the area over the scanning duration. For example, “TP-Link Smart Bulbs” and “HP OfficeJet” printers appeared. Additionally, numerous other named wi-fi networks were seen. Neither of these findings were surprising since they were likely from other nearby apartment residents.
