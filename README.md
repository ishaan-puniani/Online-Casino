# Online-Casino
Online Casino is a platform to host casino games and make them available over the network.  
There are the following components 

# Components
## GamePlatformServer [ ![Codeship Status for ishaan-puniani/GamePlatformServer](https://codeship.com/projects/f1ba8260-c8f9-0133-330b-5ee1f71ea423/status?branch=master)]
## GameExecutionServer [ ![Codeship Status for ishaan-puniani/GameExecutionServer](https://codeship.com/projects/5c27aa00-c9a8-0133-7196-6262fcd1b2c0/status?branch=master)]
## Slot_Server [ ![Codeship Status for ishaan-puniani/Slot_Server](https://codeship.com/projects/794088b0-c824-0133-6a7a-4ac43df0202f/status?branch=master)]
## Slot_Client [ ![Codeship Status for ishaan-puniani/Slot_Server](https://codeship.com/projects/a1faeed0-c8ec-0133-9841-06c431dd0dcf/status?branch=master)]

# Initial Design
![Initial Design](./InitialDesign.png?raw=true "Initial Design")



## Create Applications on OpenShift
rhc app create platform nodejs-0.10 mongodb-2.4 --noprompt --no-git NODE_ENV=production
rhc app create gameserver nodejs-0.10 mongodb-2.4 --noprompt --no-git NODE_ENV=production
