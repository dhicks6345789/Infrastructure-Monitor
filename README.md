# Infrastructure-Monitor
A Python script to monitor devices on a network.

Original code from a [project by Browolf](https://github.com/browolf/Infrastructure-Monitor).

Written to spot issues with services on a network rather than having to wait for users to report.

This code has been changed considerably from its original form. The original was a [Flask](https://flask.palletsprojects.com/en/2.2.x/) project, this version is modified to run using the [Web Console](https://github.com/dhicks6345789/web-console) project.

When run, the script reads config data from a settings file in CSV / Excel format - an example can be found [here](https://docs.google.com/spreadsheets/d/15RAP-wTBTztWJ8Z-faK-SIuat1vutkj1BQAJLpSDyxU/edit?usp=sharing). It scans the machines listed in the config file and produces an output HTML file that is then displayed.

A live example can be found [here](https://dev.sansay.co.uk/view?taskID=infrastructure-monitor).
