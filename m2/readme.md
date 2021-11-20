Part 1. 

Q: What are the most popular hypervisors for infrastructure virtualization?

A: They are Oracle VM Virtual box, VMWare vSphere, MS Hyper-V

Q: Briefly describe the main differences of the most popular hypervisors

A: There are 2 types of hypervisors:

![](images/type-hv.png)

 Type 1: hypervisor runs directly on the host machine's physical hardware:
    
	VMware ESXi
	Proxmox Virtual Environment
	Microsoft Hyper-V
	open source KVM
	Citrix Hypervisor

  Type 2: hypervisor is installed on top of an existing OS:
    
	VMware Fusion
	Oracle VM VirtualBox
	Parallels Desktop
	VMware Workstation
	VMware Player
	Microsoft Hyper-V
	Windows Virtual PC

Part 2. Work with Virtual box

I installed Virtual box on Ubuntu Desktop (main host) and downloaded latest stable version UbuntuServer (20.04). Then created VM1 and installed Ubuntu

![](images/1.4.png)
![](images/1.6.png) 
![](images/1.7.png)
![](images/1.8.png)
![](images/1.9.png)
![](images/1.9-1.png)
![](images/2.1.png)
![](images/2.2.png)
![](images/2.3.png) 

| Connection                | Ping |   |
|---------------------------|------|---|
| VM1 <\-> VM2 \(Bridged\)  | \+   |   |
| Host<\->VMs \(Bridged\)   | \+   |   |
| Host to VM\(NAT\)         | \-   |   |
| VMs\(NAT\) to internet    | \+   |   |
| VMs\(Bridge\) to internet | \+   |   |
| VMs\(Bridge\) to host     | \+   |   |
| VMs\(NAT\) to host        | \+   |   |


Then work with CLI through VBoxManage:

![](images/2.4Bridge.png)
![](images/3.2.png)

