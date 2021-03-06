
<head>
<meta name="keywords" content="python, share, connection, access point, share connection, hostapd, ethernet, wifi, ethernet through wifi, wifi through ethernet, python script, configure access point, debian, linux, wireless" >

#  connshare a python script that helps to configure simple access point 
</head>

<body>

### Introduction

**connshare** is a python script that helps to setup an access point, to share connection from one interface to another one.

For example if your machine have two interfaces: 
* eth0 wich is used with ethernet cable
* wlan0 wich is used for wifi

and suppose you want to share connection from ethernet to wifi. Cocoshare help you all the way.

### Dependencies 

* hostapd
* netfilter-persistent
* isc-dhcp-server

### Requirement

connshare has been tested on Python 2.7.

### Usage 

After installing the dependencies, run as root:
   
```python connshare```

Next it will check for dependencies, and for available interfaces, you have to choose the source and destination interface.
After that, connshare will give you a custom configurations to add to some config files like:
* /etc/default/hostapd
* /etc/default/isc-dhcp-server
* /etc/dhcp/dhcpd.conf

It also runs some commands to help you during this process. All the commands executed will be prompted to the shell. 

<img src="/imgs.gif" alt="use" align="middle" style="width:128px;height:128px;">
</body>


