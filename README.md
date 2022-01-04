3proxy install script for Debian / Ubuntu VPS
======================================================

A simple script to install 3proxy on Ubuntu/Debian

**MANUAL :**

Install :

    wget --no-check-certificate https://raw.github.com/jhuyvu/3proxy/master/3proxyinstall.sh
    chmod +x 3proxyinstall.sh
    ./3proxyinstall.sh

Change authentication!!! 

    vim /etc/3proxy/.proxyauth
	
Sample .proxyauth

    johndoe:CL:johndoepassword123

Change HTTP/SOCKS port, default 31415 (SOCKS)

    vim /etc/3proxy/3proxy.cfg
    

Start service (or reboot as it's automatically start)

    /etc/init.d/3proxy start
Or
    service 3proxy start

Restart
    
    /etc/init.d/3proxy restart

Stop
        
    /etc/init.d/3proxy stop
	
Uninstall:

	wget --no-check-certificate https://raw.github.com/jhuyvu/3proxy/master/3proxyuninstall.sh
	chmod +x 3proxyuninstall.sh
	./3proxyuninstall.sh