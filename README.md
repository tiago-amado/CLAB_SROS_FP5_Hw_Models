
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



## SR-1 FP5 models

This lab contains the six SR-1 FP5 variants. Use the comand below to deploy the lab:


```bash
# deploy a lab
clab deploy --topo hw_models_FP5_SR-1.yml
```



## SR-s FP5 models

This lab contains the SR-s FP5 variants (SR-1Se/2Se/7/14). Use the comand below to deploy the lab:

```bash
# deploy a lab
clab deploy --topo hw_models_FP5_SR-s.yml
```


## Conclusion

This is a very simple lab with distinct SROS FP5 examples with basic configs.
The purpose is to provide a quick start lab to play with MD-CLI or to be used as a reference to deploy other labs with FP5 nodes.
Please refer to the Nokia user guides (vSIM installation guide) and release notes for more details.
To build your own lab setup you need to define the required endpoints.

