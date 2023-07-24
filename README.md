
# CLAB SROS FP5 HW models: SR-1 and SR-s

These CLAB yml files provides Nokia SROS FP5 Hw Models examples.
These lab contains only examples and basic configs for a quick start playing with MD-CLI or to be used as reference for other lab setups with FP5 nodes.
It is assumed that you're familiar with Container Lab and SROS vSIMs. Refer to https://containerlab.dev/


## Clone the git lab to your server

You may simple use these files to build your own lab or clone these labs to your server and run as is. 
To deploy these labs, you should clone these labs to your server with "git clone".

```bash
# change to your directory
cd /home/user/github/
# Clone the lab to your server
git clone https://github.com/tiago-amado/CLAB_SROS_FP5_Hw_Models.git
```


## License file

SROS vSIMs require a valid license. You need to get a valid license from Nokia and place it in the "r23_license.lic" file.
```bash
# Copy/paste the license to the "r23_license.lic" file
cd CLAB_SROS_FP5_Hw_Models/
vi r23_license.lic
```


## SR-1 FP5 models

This lab contains the six SR-1 FP5 variants:

•	SR-1-24D

•	SR-1-48D

•	SR-1-46S

•	SR-1-92S

•	SR-1x-48D

•	SR-1x-92S


Use the comand below to deploy the lab:


```bash
# deploy a lab
cd CLAB_SROS_FP5_Hw_Models/
clab deploy --topo hw_models_FP5_SR-1.yml
```



## SR-s FP5 models

This lab contains the SR-s FP5 variants (SR-1Se/2Se/7/14):

•	SR-1Se

•	SR-2Se

•	SR-7s (FP5 chassis with FP4 (xcm-7s-b))

•	SR-14s (FP5 only)


Use the comand below to deploy the lab:

```bash
# deploy a lab
cd CLAB_SROS_FP5_Hw_Models/
clab deploy --topo hw_models_FP5_SR-s.yml
```

## Accessing the network elements

Once the lab has been deployed, the different SROS nodes can be accessed via SSH through their management IP address, given in the summary displayed after the execution of the deploy command. 
It is also possible to reach those nodes directly via their hostname, defined in the topology file. 

```bash
# List the containers
clab inspect -a
# reach a SROS node via SSH
ssh admin@clab-clab-hw_models_FP5_SR-1-SR-1-24D
```

## Conclusion

This is a very simple lab with distinct SROS FP5 examples with basic configs.
The purpose is to provide a quick start lab to play with MD-CLI or to be used as a reference to deploy other labs with FP5 nodes.
Please refer to the Nokia user guides (vSIM installation guide) and release notes for more details.
To build your own lab setup you need to define the required endpoints.

