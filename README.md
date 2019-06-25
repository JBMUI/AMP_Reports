Cisco AMP Categorization & Report Generator 
By Jacob Barone

Used for generating reports and categorizing threats with data taken from a Cisco AMP API. 

*** Requirements ***
This project will require:

-Python 3.7 or a compatible version (See Starting Off)
-xlsxwriter, regex, dateutil and requests modules (See Starting Off)
-Microsoft Excel

*** Starting Off ***

Download Python 3.7 or above here ---> https://www.python.org/downloads/
-Follow the installation guide

To get the required modules simply use the following commands within the Terminal/Command Line:

' pip install xlsxwriter '
' pip install regex '
' pip install python-dateutil '
' pip install requests '

*Note if using Windows OS simply add ' py -m ' to the beginning of each command. 

*** Formatting Requests ***

When prompted for a start/end date please note that following:

-Dates must be in the YYYY-MM-DD format. 
-Start Date indicates the beggining of the data.
-Start Date will have a time of 00:00:00+00:00
-End Date indicates the ending of the data.
-End Date will have a time of 23:59:59+00:00

*** Common Issues ***

- You should not have your End Date equal to the current date. Doing so will not query all results
for a day, as not all of the events have occured. 

- If you select a time frame that is too short (Less then 10 events total) you will recieve the
following error:

IndexError: list index out of range


