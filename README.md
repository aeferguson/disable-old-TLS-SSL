# disable-old-TLS-SSL

This is a script which when run locally on a Windows Server will update the registry entries and disable the out of date and insecure protocols TLS 1.0, TLS 1.1, SSL 2.0, and SSL 3.0.
This has been tested on Windows Server 2016 Standard 64-bit with IIS. There are no parameters needed to run this script. It outputs a log file on the users desktop.

Some things to keep in mind:

* It would be in your best interest to make a full backup of the registry before changing any values, especially scripted.
* You should have full admin access to server if you want to run this script.
* Check your ExecutionPolicy in Powershell before running this as a script (Get-ExecutionPolicy).
* After this script runs, you should reboot the server to apply the registry changes.
* Run this script at your own risk. 

## Authors

* **Andrew Ferguson** - *Initial work* - (https://github.com/aeferguson)

## License
This project is licensed under the [GNU-GPLv3](https://www.gnu.org/licenses/gpl-3.0) License - see the [LICENSE.md](LICENSE.md) file for details\
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)