# fuckForticlient

**fuckForticlient** is a command-line utility to connect to SAML fortivpn servers by using **openfortivpn** and the --cookie-in-stdin parameter.
This repo was formerly a [Github gist](https://gist.github.com/nonamed01).

# Usage

```
   ___         __    ____         __  _     ___          __         
  / _/_ ______/ /__ / __/__  ____/ /_(_)___/ (_)__ ___  / /_        
 / _/ // / __/  '_// _// _ \/ __/ __/ / __/ / / -_) _ \/ __/        
/_/ \_,_/\__/_/\_\/_/  \___/_/  \__/_/\__/_/_/\__/_//_/\__/  v1.1 

2022-2023 by: Toni Castillo Girona (@Disbauxes) 

[*] Detected distro: Debian, version: 12 
[*] Auto-detected firefox profile: /home/user/.mozilla/firefox/vujtoola.default/sessionstore-backups 
[*] Openfortivpn version: 1.20.5 
[*] Openfortivpn installed from: GITHUB 

Usage: fuckForticlient.sh  -L|-u|-d|[-p][-P][-t][-v][-S][-c][-s]  
 	-h Shows this help and exits.   
 	-c Opens firefox to perform SAML Authentication. 
 	-s Tries to re-use a previous SVPNCOOKIE.   
 	-p PATH Overrides the detection of the Firefox Profile to use. 
 	-P Saves chosen Firefox Profile (-p) as the default one.    
 	-t SECONDS Sets the timeout to wait for the SVPNCOOKIE cookie to SECONDS. 
 	-v Shows the SVPNCOOKIE cookie on screen.   
 	-S SERVER Authenticates against VPN server SERVER . 
 	-L Lists all Firefox profiles detected and exits.   
 	-d Removes Forticlient from the system and exits.   
 	-u Updates openfortivpn and exits.  
 	-i Shows current assigned VPN Ip address and exits.    
 	-D Runs the script in debug mode.   
 Examples:  
 	fuckForticlient.sh -L 
 	fuckForticlient.sh -S myserver.org.edu -c 
 	fuckForticlient.sh -i   
 	fuckForticlient.sh -t 200 -S myvpnserver.com -c  
 	fuckForticlient.sh -p /home/u1/.mozilla/firefox/myprofile -S vpnsrv -c 
 	fuckForticlient.sh -p /home/u1/.mozilla/firefox/myprofile -P -S vpnsrv -c   
 	fuckForticlient.sh -p /home/u1/.mozilla/firefox/myprofile -S vpnsrv -s  
 	fuckForticlient.sh -t 200 -p /home/u1/.mozilla/firefox/myprofile -S vpnsrv -c 

 Extra options for openfortivpn 
 	 FUCKFORTICLIENT_OPTS="--op1 --op2 ..." fuckForticlient.sh options ...  
 Example:   
 	FUCKFORTICLIENT_OPTS="--no-dns" fuckForticlient.sh -S myserver.org.edu -c 

```
