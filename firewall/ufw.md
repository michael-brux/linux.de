## ufw UncomplicatedFirewall

### vor dem Einschalten
mit dem aktivieren von ufw wird eine Remote Verbindung (via ssh) möglicherweise unterbrochen
#### daher vorher:
- prüfen, welche default policy (allow/deny) gilt:
``` 
grep "POLICY" /etc/default/ufw
```
- prüfen, ob ssh durch eine Regel erlaubt ist:  
```
ufw show added
```
#### Quellen / Links

[Projektseite im Ubuntu wiki](https://wiki.ubuntu.com/UncomplicatedFirewall)   
[Communitiy Documentation](https://help.ubuntu.com/community/UFW)   
[Ubuntu Server Guide](https://ubuntu.com/server/docs/security-firewall)  
[ufw man page - Ubuntu 20.04](http://manpages.ubuntu.com/manpages/focal/en/man8/ufw.8.html)  
[ufw-framework man page - Ubuntu 20.04](http://manpages.ubuntu.com/manpages/focal/en/man8/ufw-framework.8.html)    
[Launchpad: ufw](https://launchpad.net/ufw/)  
[Debian wiki](https://wiki.debian.org/Uncomplicated%20Firewall%20%28ufw%29)  
[Tutorial DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-firewall-with-ufw-on-ubuntu-20-04)  
[Debian Package Tracker](https://tracker.debian.org/pkg/ufw)  
