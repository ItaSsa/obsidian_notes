## Groups on Linux
	- Checking all groups : `cat  /etc/group` 
	- Groups from user: `groupsgt`
	- Adding group: `sudo addgroup ubuntu`
	- Creating a new user: `sudo adduser linux`
	- Adding a user to a group:  
		-`sudo adduser linux ubuntu`
			`sudo gpasswd -a itaira teste`
	- Changingm user: `su linux`
	- Removing a user from a group: `sudo gpasswd -d itaira ubuntu`
	- Removing a group: `sudo groupdel ubuntu`

## Permissions
	- show details : `ls -lh`
		owner / group / others

	- changing permissions: `chmod ` 
	 ![[Pasted image 20250507081402.png]]
	 

## Compactors
 - gzip -
	 - Maxi compactatio tax: gzip -9 file_name
 - gunzip
 - zip name.zip filename.txt
 - unzip filename.zip
 - bzip2 file
 - bzip2 -d file
 - rar a file.rar file
 - rar x file.rar
 
## Archiver
- tar -cf file.txt.tar  file.tar
- Compacting a tar file: `gzip files.tar`
-  Unzip: `tar -xvf files.tar.gz
		`tar  -xvf files.tar.gz -C ~/newLocal`

## Comands
- Cleaning History: `history -c
- `alias hh='history'`
- Counting lines: `wl file`
	- `wc -l file.txt`
- Counting words: `wc -w file.txt"
- Counting number of `caracters: wc -m file.txr  
- Comparing files: `cmp file1 file2`
- `diff`file1 file2`
- `sort -m file`
- Reboot info: `last reboot`
- `route -n`
- `time traceroute www.google.com`
- uptime
- Let the cow say: `cowsay message`
	- `cowsay -f tux teste`
	  `cowsay -f vader teste`
	- `cowsay -f vader-coala teste`
	- `cowsay -f dragon teste`
	- xcowsay "I'm in colors"
- `cmatrix 

## Machine commands
- halt
- range:  `seq 1 10`

## Packages

- apt: 
	- `sudo apt install nmap`
	- `sudo apt upgrade nmap`
	- `sudo apt remove nmap`
- dpkg
	- Install: `sudo dpkg -i package_name.deb`
	- Get info: `sudo dpkg -I package_name.deb`
	- remove: `sudo dpkg -r package_name_via_description `
- rpm (on Fedora)
	- rpm -ivh package.ext
	- Without dependences: rpm -ivh --nodeps package.ext
	- Upgrade: sudo rpm -U pack_name
	- removing: sudo rpm -e pack_name
- yum (Fedora)
	- Download and install: sudo yum install pack_name
	- Update:  sudo yum update pac_name
	- Remove: sudo yum remove pac_name
- System upgrade
	- `apt update && apt upgrade`
	- Sites:
		- pkgs.org
		- 