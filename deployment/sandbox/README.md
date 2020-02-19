# MOSIP Sandbox Deployer
  
Enables the creation of MOSIP sandbox on a Linux OS.  Using pre-crafted docker images, it enables one to quickly setup MOSIP for trying and demonstrating. THIS IS NOT FOR PRODUCTION DEPLOYMENTS.  

## Overview
![](images/sandbox-overview.png)

## Pre-requisites
This has been tried and verified 
      * OS : Ubuntu 18.0.4 LTS
      * Hardware : 4 core CPU with 32 GB RAM and a about 200 GB of free hard disk space.
      * Make sure you have installed 'curl' and 'git'
      
## Get, Set, Go!
1. Clone the 'mosip-infra' repo
      $ git clone https://github.com/mosip/mosip-infra

1. Edit `mosip-infra/deployment/sandbox/playbooks-properties/all-playbooks.properties` with appropriate values (Change only \<ToBeReplaced\>)

1. Change over to 'sandbox' folder which has the shell scripts for installing various MOSIP components
     $ cd ~/mosip-infra/deployment/sandbox/

1. Install the MOSIP Kernel *****Pre-requisite for installing other modules
     $ sudu sh install-mosip-kernel.sh
     
#### Pre-registration 
     $ sudo sh install-mosip-pre-reg.sh
     
     * Check for successful installation
     ** From any browser, type 'https://<hostname or ip address>/pre-registration-ui'

#### Registration Processor

#### Install ID Authentication

#### Install ID Repo

