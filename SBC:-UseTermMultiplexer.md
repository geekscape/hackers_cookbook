# Summary

Avoid the overhead of running a graphical user interface on small systems and resume working after losing connection to remote system.

# Usage

## Issue Addressed

1. Often connections to a remote embedded device will drop out and any work will be lost
2. Running X Windows on a Rspberry Pi loads the system and is more complicated to access remotely.

## Solution

Install and use termnial multiplex on a Raspberry Pi. There are two choices. GNU Screen and tmux. If you are using an small embedded device (e.g.) and Arduino
then consider installing a Raspberry Pi to support a terminal multiplexer if and as needed.

The following instructions assume you are tmux with the default keymapping on a Raspian GNU/Linux system to which you are connecting

1. Install the tmux package ``sudo apt-get update && sudo apt-get install -y tmux``
2. Login to the Raspberry Pi from a workking terminal connection (via LAN or serical console)
3. Run the command ``tmux``
4. Type commands as normal

If you loose you connection to the device then simply reconnet and issue the comannd ``tmux attach``. You are returned to your session and carr on where you left off

###Multiple panes

In the following the default prefix is <ctrl-b>

* To split the terminal screen in half vertically press <prefix>%
* To split the terminal screen in half vertically press <prefix>"
* To move to the next pane press <prefix>o
* To close down tmux exit each pane with ``exit`` or <ctrl-d>

There are many other features in both tmux and screen. However these basics will get you started. Consult the manual for more information.



# References

[GNU Screen Home Page](http://www.gnu.org/software/screen/)
[tmux Home Page](http://tmux.sourceforge.net/)


<a rel="license" href="http://creativecommons.org/licenses/by-nc/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">OSHCB</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/3.0/deed.en_US">Creative Commons Attribution-NonCommercial 3.0 Unported License</a>.
