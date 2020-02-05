# Django-ChatAPP

Need to run a redis server at <b>127.0.0.1:6379</b> to properly implement the app

## In Order to run a redis server on windows, Windows Subsystem for Linux (WSL) can be used

1.To enable Windows Subsystem for Linux, follow the instructions on Microsoft Docs. The short version is: In Windows 10, Microsoft replaces Command Prompt with PowerShell as the default shell. Open PowerShell as Administrator and run this command to enable Windows Subsystem for Linux (WSL):
```bash
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```
2.Reboot Windows after making the change—note that you only need to do this one time.

3.Download and install one of the supported Linux distros from the Microsoft Store.

## Now to run Redis Server

1.Launch the installed distro from your Windows Store and then install redis-server. The following example works with Ubuntu (you’ll need to wait for initialization and create a login upon first use):
```bash
> sudo apt-get update
> sudo apt-get upgrade
> sudo apt-get install redis-server
> redis-cli -v
```
2.Restart the Redis server to make sure it is running:
```bash
> sudo service redis-server restart
```
3.Execute a simple Redis command to verify your Redis server is running and available:
```bash
$ redis-cli 
127.0.0.1:6379> set user:1 "Jane"
127.0.0.1:6379> get user:1
"Jane"
```
4.To stop your Redis server:
```bash
> sudo service redis-server stop
```



