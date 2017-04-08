# shell-tool-box
A set of miscellaneous shell scripts that doing miscellaneous tasks.

###IP Selector([ipselector](ipselector))
```sh
Usage:
    ipselector [-d|--debug] [-p|physical] [-a|--actived] [-m [prompt text]|--message[=prompt text]]
    -d | --debug     enabling debug model
    -p | --physical  only select physical network card
    -a | --actived   only select actived(which is up and running) network card
    -m | --message   the prompt text to shown when need user to select one ip
Example:
    $name -p -m "Please chose an IP for Tomcat:"
```
