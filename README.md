# vmware-vm-creator

## Description
Simple utility to create vm in vcenter using pyvmomi from vmware  
Also a little simple utility to list vms in vcenter together with some properties

## Installation
First you need the pyvmomi  
pip install pyvmomi  
You need login info and to know a little bit about what you are doing. I do not
recommend using this if you are not experienced and already know what you are
doing. Rock and roll

## Usage vmware-vm-creator
*vmware-vm-creator --help  
usage: vmware-vm-creator [-h] [-V--vcenter VCENTER] [-u--user USER]  
                         [-n--vm_name VM_NAME] [-r--memoryMB MEMORYMB]  
                         [-c--numcores NUMCORES] [-d--disksize DISKSIZE]  

Virtual machine creator.  

optional arguments:  
  -h, --help            show this help message and exit  
  -V--vcenter VCENTER   vcenter to connect to  
  -u--user USER         vcenter login  
  -n--vm_name VM_NAME   short vm_name (without domainpart)  
  -r--memoryMB MEMORYMB  
                        Memory for the vm in GB  
  -c--numcores NUMCORES  
                        Number of cores  
  -d--disksize DISKSIZE  
                        Disksize in GB  


## Usage vmlister  
vmlister <partialhostname>  
  
Name:              partialhostname.domain.com  
Vcenter:           vcenter00.domain.com  
Power:              poweredOn  
Guest:             Red Hat Enterprise Linux 7 (64-bit)  
Path:              [superstorage] partialhostname.domain.com.vmx  
Memory (Ram MB):   8192  
Num cpu:           4  
Network Up: 10.1.2.30-24  
Storage Commited: 144.2 GB ; Uncommited 0.0 GB  
Esx Host:  esxhost-x.domain.com  

