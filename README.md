# Shell Tool Box
A set of miscellaneous shell scripts that doing miscellaneous tasks.

### IP Selector([ipselector](ipselector))
    Let the user to determine which ip address to use for some purpose. The network card(virtual or physical ones) which is not up will be assigned an address of "0.0.0.0".

**Usage:**
```sh
ipselector [-d|--debug] [-p|physical] [-a|--actived] [-m [prompt text]|--message[=prompt text]]
-d | --debug     enabling debug model
-p | --physical  only select physical network card
-a | --actived   only select actived(which is up and running) network card
-m | --message   the prompt text to shown when need user to select one ip
```
**Example:**
```sh
$ TOMCAT_IP=$(ipselector -p -m "Please chose an IP for Tomcat:")
Please chose an IP for Tomcat:
1) p4p1                0.0.0.0
2) wlan0               192.168.1.1
#? 2
$ echo $TOMCAT_IP
192.168.1.1
```

