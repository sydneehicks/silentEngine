.. SPDX-License-Identifier: AGPL-3.0-or-later

.. figure:: https://github.com/sydneehicks/silentEngine/blob/master/searx/static/themes/silent/img/silent.png
   :target: https://searx.github.io/searx/
   :alt: searX
   :width: 100%
   :align: center

-------

A privacy metasearch engine powered by searx.


- Self-hosting
- Customizable (using preferences)
- No tracking
- Uses over 70 search engines

----------------------------------
Recommendations before installing:
----------------------------------

- Use a Ubuntu 20.4 or newer computer.
- Change root password with the following command:
    - sudo passwd root
- If any commands do not work, change user to root:
    - su root
    - Enter password
- Make sure that the following packages are installed:
    - Pyyaml
    - python-dateutil
    - dateutil.parser
    - httpx
    - Flask
    - Babel 
    - Flask_babel
    - pygments
    - werkzeug
    - h2
    - uvloop
    - httpx_socks
    - lxml
    - langdetect

--------------------------
Installation Instructions:
--------------------------
- Open Terminal 
==================
Check for updates:
==================

Run the command:
- sudo apt-get update –y

=====================
Download dependencies
=====================

Run the command:
-sudo apt-get install git build-essential python-babel zlib1g-dev libffi-dev libssl-dev libxslt-dev python-dev python-virtualenv -y

- If you get a message: “Package python-virtualenv has not installation candidate”
   * Run the following commands:
      * sudo apt-get update
      * sudo apt-get install python3-virtualenv
   And python-virtualenv will be installed.

=====================
Install SilentEngine
=====================

- Change the directory to where you would like SilentEngine to be stored
   * cd <directory name>
- Clone the GitHub repository:
   * sudo git clone https://github.com/sydneehicks/silentEngine.git

==================
Tip:
==================

- go to .../SilentEngine/settings.yml
- change the secret key! SilentEngine will not run unless the secret key is change from “ultrasecretkey”. You can create your own add it in the file!

=====================
Launch SilentEngine
=====================

- run the following command to run SilentEngine!
	python3 searx/webapp.py

--------------------------
References:
--------------------------

- SearX github: https://github.com/searx/searx.git
- how to install SearX on Ubuntu: https://vitux.com/how-to-install-searx-search-engine-on-ubuntu/
