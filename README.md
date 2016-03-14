# Online-Casino
Online Casino is a platform to host casino games and make them available over the network.  
There are the following components 

# Components
## [GamePlatformServer](http://platform-gameolive.rhcloud.com/) [ ![Codeship Status for ishaan-puniani/GamePlatformServer](https://codeship.com/projects/f1ba8260-c8f9-0133-330b-5ee1f71ea423/status?branch=master)]
[Demo](http://platform-gameolive.rhcloud.com/)
## [GameExecutionServer](http://gameserver-gameolive.rhcloud.com/) [ ![Codeship Status for ishaan-puniani/GameExecutionServer](https://codeship.com/projects/5c27aa00-c9a8-0133-7196-6262fcd1b2c0/status?branch=master)]
[Demo](http://gameserver-gameolive.rhcloud.com/)
## Slot_Server [ ![Codeship Status for ishaan-puniani/Slot_Server](https://codeship.com/projects/794088b0-c824-0133-6a7a-4ac43df0202f/status?branch=master)]
## Slot_Client [ ![Codeship Status for ishaan-puniani/Slot_Server](https://codeship.com/projects/a1faeed0-c8ec-0133-9841-06c431dd0dcf/status?branch=master)]

# Initial Design
![Initial Design](./InitialDesign.png?raw=true "Initial Design")

# Instructions to setup 
## Prerequisites 
1. Mongodb
2. nodejs
3. grunt 
4. bower

## Setup Projects 
1. Clone [Game Platform Server](https://github.com/ishaan-puniani/GameExecutionServer)

1. npm install

2. bower intall

3. grunt serve


2. Clone [Execution Server](https://github.com/ishaan-puniani/GamePlatformServer)

1. npm install

2. bower intall

3. grunt serve




## Create Applications on OpenShift
rhc app create platform nodejs-0.10 mongodb-2.4 --noprompt --no-git NODE_ENV=production

rhc app create gameserver nodejs-0.10 mongodb-2.4 --noprompt --no-git NODE_ENV=production
