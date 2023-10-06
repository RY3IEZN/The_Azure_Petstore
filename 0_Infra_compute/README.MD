<!-- @format -->

# 0 Set up Infrastructure

In this spirit of an azure cloud engineer we will be setting up all our infrastructure on azure cloud

So without wasting anymore Sign in to the azure portal and create a VM

Search for virtual machines and click create

![](images/infra1.png)

Select Azure Virtual machine

![](images/infra2.png)

Fill in all the details as required,

**NB.All resources including network,storage will be created as we go along the creation of the vm**

![](images/infra3a.png)

i used an ubuntu OS with 2gb ram (more than enough to test and push to acr),set the username and password, leave the inbound port as 22, next disk

![](images/infra3b.png)

for disk/storage leave everything as default, dont need much

![](images/infra4.png)

same applies for networking the basics are fine, a default vpc and subnet will br created for you

![](images/infra5.png)

As for management set the shutdown time to be 10pm incase you sleep and forget the vm, leave the rest a default

![](images/infra6.png)

For monitoring, disable the boot diagnostics, we dont need that again leave the rest as default

![](images/infra7.png)

if you noticed i skipped advanced, nothing to do there, except maybe you want something to be intialised as soon as the vm is up, other than that go straight and tag your resources

![](images/infra8.png)

Review your configuration and then click create

![](images/infra9.png)

wait for it to create and then go to the resource

![](images/infra10.png)

Great we have a fresh clean ubuntu vm to use and push to docker

![](images/infra11.png)
