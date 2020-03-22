============
Installing
============

- This is a portable software, So you do not need to install this.
- Extract ``Scraper.zip`` 
- Double Click on main.exe
- It should open the software
============
Preparing Source File
============
- To use this software, you must have a source file which contains list of URL's
- Source file should be hosted as a Google spreadsheet.
- Ex -
.. image:: https://i.postimg.cc/rsT3YsgD/12.png
-Then you should share this google sheet with Google service account email address
- shanaka@sjp-fot.iam.gserviceaccount.com
.. image:: https://i.postimg.cc/Y9YT3YNc/9.png
- Please set Edit Permissions to above mentioned email address
- [NOTE] If you are using a different Service account, you should share source file with service account's email address.
- You can find Service account's email address inside service account's JSON file.
.. image:: https://i.postimg.cc/1Rp2LGk4/13.png
============
Using with Windows
============

- Open the software
.. image:: https://i.postimg.cc/SshMXbD6/10.png


- Enter Google Sheet ID. Please Note that DO NOT Enter Google Page URL
- Here is how you can find ID of google Spreadsheet
.. image:: https://i.postimg.cc/Hk5GkmsT/4.png

- Click on Load URL's Button
- It may take some time depending on size of Google Spreadsheet
- Now enter Linkedin Username and Password.
- Enter Minimum and Maximum Delays between scraping two URL's (in seconds)
.. image:: https://i.postimg.cc/ZnYvcFk0/11.png

===============
- If you do not tick this "Headless Scraping" Check box, A web browser window will be opened and scraping process will be done automatically.
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
- Find these lines in ``main.py``
1. ``driver = webdriver.Firefox(options=options,executable_path=r"./geckodriver.exe")``
2. ``driver = webdriver.Chrome(chrome_options=chrome_options,executable_path=r"./chromedriver.exe")``

- If you downloaded geckodriver, replace "./geckodriver.exe" in line 1 with "./geckodriver"
- If you downloaded geckodriver, replace "./chromedriver.exe" in line 2 with "./chromedriver"
- Run Code by pressing ``F5``
- You will get the same working software with same UI
.. image:: https://i.postimg.cc/8P7QxW2J/3.png
- Enjoy the software!

============
Remove Credits
============

- If you want to remove the line ``Developed by Shanaka Anuradha @ UpWork``
- Open "main.ui" file inside software with any text editor

- Find below text, remove it and save file.

<widget class="QLabel" name="label_8">
    <property name="geometry">
     <rect>
      <x>160</x>
      <y>440</y>
      <width>281</width>
      <height>16</height>
     </rect>
    </property>
    <property name="font">
     <font>
      <family>MS Shell Dlg 2</family>
      <pointsize>7</pointsize>
      <weight>50</weight>
      <italic>false</italic>
      <bold>false</bold>
     </font>
    </property>
    <property name="autoFillBackground">
     <bool>false</bool>
    </property>
    <property name="styleSheet">
     <string notr="true">color:rgb(43, 0, 0)</string>
    </property>
    <property name="text">
     <string>Developed by Shanaka Anuradha @ UpWork</string>
    </property>
   </widget>
============
Change Google Service Account
============
- Follow This article and create a Google Service Account
- `https://medium.com/@denisluiz/python-with-google-sheets-service-account-step-by-step-8f74c26ed28e <https://medium.com/@denisluiz/python-with-google-sheets-service-account-step-by-step-8f74c26ed28e>`_
- Download JSON file which contains authentication details
- Rename JSON file to "sjp-fot-fc1cbfbc9993.json"
- Copy JSON file to software folder.Replace exsisting one.
- Now you are ready to use your google Service account.
- Please note that you have to share source file with new Service account's email address.
- You can find Service account's email address inside JSON file.
.. image:: https://i.postimg.cc/1Rp2LGk4/13.png
