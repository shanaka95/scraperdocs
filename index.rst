============
Installing
============

- This is a portable software, So you do not need to install this.
- Extract ``Scraper.zip`` 
- Double Click on main.exe
- It should open the software
============
Using with Windows
============

- Open the software
.. image:: https://i.postimg.cc/8P7QxW2J/3.png


- Enter Google Sheet ID. Please Note that DO NOT Enter Google Page URL
- Here is how you can find ID of google Spreadsheet
.. image:: https://i.postimg.cc/Hk5GkmsT/4.png

- Click on Load URL's Button
- It may take some time depending on size of Google Spreadsheet
- Now enter Linkedin Username and Password.
- Enter a gmail Email Address. Please note that Result Google sheet will be shared automatically with this email address. So you have to be logged in to this email address for viewing result google sheet.
- Enter Minimum and Maximum Delays between scraping two URL's (in seconds)
.. image:: https://i.postimg.cc/xdSwkZcM/5.png
- Optionally Enter a name for result Google sheet.If you do not enter this, a name will be generated with current timestamp.
Headless Scraping
===============
- If you do not tick this "Headless Scraping" Check box, A web browser window will be opened and you can scraping process will be done automatically.
- You can see what is going on.
- But if you want to get rid of this browser window, Just tick on  "Headless Scraping".Then no browser Window Will be opened while scraping.
Using FireFox
===============
- FireFox is the recommended web browser for this software.
- You have to install latest Firefox WebBrowser before using this software.
- If you have installed FireFox, You do not need any other thing to do.Just Select "Use FireFox"
radio button

Using Chrome
===============
- If you need to use this software with Chrome web browser, You need to complete one extra step.
- First, Install Chrome Browser
- Find the version of chrome browser
.. image:: https://i.postimg.cc/6QBFB1j3/8.png

- Go to `https://chromedriver.chromium.org/downloads <https://chromedriver.chromium.org/downloads>`_
- Find the Chromedriver matches with your Chrome browser Version.
- If you have Chrome Browser version 80.x , Yo have to download Chrome Driver which supports Chrome Browser version 80.x
.. image:: https://i.postimg.cc/KzHWrcZk/9.jpg

- Download chromedriver_win32.zip
.. image:: https://i.postimg.cc/XJJhCB06/10.jpg

- There is a file "Chromedrive.exe" inside downloaded zip file.
- Extract it inside scraper software folder.It will ask you to replace the current file.Replace it.
.. image:: https://i.postimg.cc/kGRpjr4j/11.jpg
- Now you are ready to use the software with Chrome Browser.

Start Scraping
===============
- After filling all the required fields, Click on Start Button.
- Scraping will be started immediately

============
Using on Linux or MacOS
============

- You can run this software on Linux or MacOS using source Code
Installing Python
===============
- First You should install python 2.7 for Linux or MacOS 
- `https://www.python.org/download/releases/2.7/ <https://www.python.org/download/releases/2.7/>`_
- Then install following python modules using pip
- ``pip install <module name>``
- Example -  ``pip install pygsheets``
List of required python modules
""""""""""""""""""
1. pygsheets
2. urllib
3. json
4. PyQt4
5. selenium
6. webbrowser

Running Software
===============
- After installing Python and required modules, you can open main.py source file using python IDLE
.. image:: https://i.postimg.cc/52xKQKvF/1.png

- If you run this on Linux or MacOS you should have installed Firefox or Chrome.
- If you have installed Firefox or Chrome then you have to download suitable Chromedriver for chrome or Geckodriver for Firefox.
- GeckoDriver - `https://github.com/mozilla/geckodriver/releases <https://github.com/mozilla/geckodriver/releases>`_

- ChromeDriver - `https://chromedriver.chromium.org/downloads <https://chromedriver.chromium.org/downloads>`_
- Download the package that matches with your OS and Chrome or Firefox version.
- Then extract downloaded zip file inside the source code of software.
- 
- Run Code by pressing ``F5``
- You will get the same working software with same UI
.. image:: https://i.postimg.cc/8P7QxW2J/3.png
