# TPL-AutoRenewal

This script automatically renews your Toronto Public Library (TPL) checkouts the day before they're due

If for some reason the checkouts could not be renewed, you will receive an email notification of the error

Please star this repo if it's helped you

## Setup (~8 minutes)

### Download this repo

Download this repo

### Install Python 3

Install [Python 3](https://www.python.org/downloads/) on your machine


### Install Selenium

Run the following command in your terminal

pip install -U selenium
<br><br>

### Enter your own authentication credentials

Open auth.txt

Replace the word PLACEHOLDER with your respective credentials
<br><br>

### Set the script to run automatically (Windows) - Video

This video shows you how to use TaskScheduler to automatically run a Python script: https://www.youtube.com/watch?v=n2Cr_YRQk7o

Make sure you set the 'Add arguments' field to 'TPL-AutoRenewal.py'

Make sure you set the 'Start in' field to the installation location of this repo  

Example: 'C:\Users\USERNAME\Downloads\TPL-AutoRenewal'

Replace USERNAME with your computer's username
<br><br>

### Set the script to run automatically (Windows) - Text

Open TaskScheduler

On the right hand side, click 'Create Task'


<br><br>
In the Name field type 'TPL-AutoRenewal'

Click the radio button labelled 'Run whether user is logged on or not'


<br><br>
On the top, click the tab labelled 'Triggers'

Click the button labelled 'New'

A window will pop up, click daily on the left hand side

Click 'OK' in the bottom right

<br><br>
On the top, click the tab labelled 'Actions'

Click the button labelled 'New'

In the input field labelled 'Program/script' paste the fullpath to your Python installation location

The default location is 'C:\Users\USERNAME\AppData\Local\Programs\Python\Python36'

Replace USERNAME with your computer's username

In the input field labelled 'Add arguments' type 'TPL-AutoRenewal.py'

In the input field labelled 'Start in' paste the location of where you downloaded this repo

Example: 'C:\Users\USERNAME\Downloads\TPL-AutoRenewal'

Replace USERNAME with your computer's username


<br><br>
On the top, click the tab labelled 'Conditions'

Make sure the checkbox labelled 'Start the task only if the computer is on AC power' is unchecked

Check the checkbox labelled 'Wake the computer to run this task'

Check the checkbox labelled 'Start only if the following network connection is available'

Set the dropdown to 'Any connection'


<br><br>
On the top, click the tab labelled 'Settings'

Check the checkbox labelled 'Run task as soon as possible if a scheduled start is missed'


<br><br>
On the bottom click 'OK'

Enter your windows password


<br><br>
Your library checkouts will now be automatically renewed the day before they're due!
<br><br>

### Set the script to run automatically (macOS)
In your terminal type

crontab 0 1 * * * /path/to/script

Replace /path/to/script with the actual path to TPL-AutoRenewal.py
