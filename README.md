# DevOps_297: Minecraft Server 
Contributors: [Matthew Ingenito](https://github.com/ingenitom)
and [Jorge Aguilar](https://github.com/Jav-aguilar)

## Overview
This goal of this project was to create a Minecraft spigot server that has been modified with added plugins. Also to be able to run the server locally on your laptop, on a virtual machine (Docker or Vagrant) on your laptop, and finally on a cloud-hosted machine(Heroku or AWS). 

## Setup
1. Fork this repo
2. Copy your forked repo url
3. Create a directory to store the forked repo: `mkdir <name_directory>`. 
4. Then cd into that directory: `cd <name_directory>`
5. then clone the forked repo: `git clone <forked_repo_url>`
6. run `ls` on the command line to make sure the repo is in the directory

### Locally
1. Cd into the `Working_MC_Server` by doing `cd DevOps297_final/Working_MC_Server/`
2. Then launch the Minecraft Spigot Server: `java -Xmx1G -Xms1G -jar server.jar nogui`
3. To stop the server on the terminal comand line type `stop` and then enter

### Vagrant 
1. Check to make sure you are in the directory `Working_MC_Server` by running `pwd`
2. If not, cd into the `Working_MC_Server` by doing `cd DevOps297_final/Working_MC_Server/`
3. Type `vagrant up` to launch the Minecraft Spigot Server
4. To stop the server on the terminal comand line type `stop` and then enter
5. Then `vagrant destroy` to destroy the virtual machine


### AWS (Amazon Web Services)
1. Launch your AWS Lightsail instance
2. Configure and Connect to your instance
3. In "Networking" add a firewall rule to allow port `25565`
4. Tab over to the connect tab and select ` Connect using SSH`
5. Enter this command that updates the serverand installs JavaRuntime: `sudo apt -y update && sudo apt -y install default-jre screen`
6. Clone the repo with `git clone <repo_url>`
7. Cd into the correct directory: `cd DevOps297_final/Working_MC_Server/`
8. Run `sudo java -Xmx1G -Xms1G -jar server.jar nogui`



## Technologies Used
1. [Ruby](https://www.ruby-lang.org/en/)
2. [Vagrant](https://www.vagrantup.com/)
3. [AWS](https://aws.amazon.com/)

## Helpful Resources
-  [Create Minecraft Spigot Server tutorial](https://www.youtube.com/watch?v=WaHWgNwcBh8)
	- [Spigot Server download](https://getbukkit.org/download/spigot)
	- [Java download](https://www.java.com/en/download/manual.jsp)
-  [AWS tutorial](https://www.youtube.com/watch?v=Iv13FrZCdko)
-  [List of plugins for Minecraft Server](https://thebreakdown.xyz/top-10-plugins-for-bukkit-spigot-servers/)
	- [EssentialsX ](https://www.spigotmc.org/resources/essentialsx.9089/)
	- [Holographic Displays ](https://dev.bukkit.org/projects/holographic-displays)
	- [WorldEdit](https://dev.bukkit.org/projects/worldedit)


