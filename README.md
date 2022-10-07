# Infrastructure-Monitor
A Python script to monitor devices on a network.

Original code from a [project by Browolf](https://github.com/browolf/Infrastructure-Monitor).

Written to spot issues with services on a network rather than having to wait for users to report.

It uses Flask which can be installed with Pip. https://www.w3schools.com/python/python_pip.asp
If you have smoothwall, certificate errors can be stopped by excluding the pypi urls from https inspection.

I run the script as a service on an ubuntu server plugged into the core switch. We also have port forwarding on smoothwall so it's accessible from outside. 
At the moment it displays on a pc/ monitor in our office but planning to get a smart tv on the wall instead. The script works equally well on windows server or 10.

You may wonder why it shows iterations on the page - the previous version that worked differently had an issue where it could stop working and you couldn't tell. 
The number represents every time the page is generated on the server so if the number is going up it's definitely working. 
It has a 10 second refresh which is specified in the html file.

It checks open ports of devices which you can find with nmap. On windows servers I'm using the rdp port 3389
