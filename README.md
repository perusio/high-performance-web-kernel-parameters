# High performace web server setup

## Introduction

This is a set of configuration files for the Linux kernel that allow
to setup a high-performance web server and accompanying DB server.

It follows the debian setup where there's a directory `/etc/sysctl.d`
where you place **all** your kernel configuration parameters files
with names descriptive of which subsystem of the kernel it relates to.

## Installation

 1. Clone the repo:
        
        git clone git://github.com/perusio/high-performance-web-kernel-parameters.git 

 2. Choose the configuration based on the type of role that your
    server will play **web server** or **DB server**.

 3. Copy from the directory `webserver` (for web servers) to
    `/etc/sysctl.d`.
    
    Copy from the directory `dbserver` (for DB servers) to
    `/etc/sysctl.d`  

 4. Update the kernel config using:
        
        sysctl --system
        
 5. Done
 
Note that from now on, this configuation will be used for setting the
kernel parameters at boot time.
  
## TODO
 
Improve the documentation. Add Intel paper discussion for better understanding.
