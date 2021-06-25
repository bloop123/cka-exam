# Node Upgrades
Cordon Node: Mark a node unschedulable
`kubectl cordon <nodename`
Drain Nodes:
`kubectl drain node <nodename>` : drain and uncordon

## kubernetes version Upgrade
![image](https://user-images.githubusercontent.com/17488415/123371966-51df3b80-d5a0-11eb-8206-610ccb132be0.png)
![image](https://user-images.githubusercontent.com/17488415/123371999-61f71b00-d5a0-11eb-8ee9-616d6a9489fd.png)

deployable kubenernetes package contains all components at same version
![image](https://user-images.githubusercontent.com/17488415/123376623-6a535400-d5a8-11eb-93ec-89cd8af99fd2.png)


All internal deployed components may not have same version. 

allows us to upgrade each component independently.
![image](https://user-images.githubusercontent.com/17488415/123376835-c4ecb000-d5a8-11eb-8eec-a4b06de87665.png)

Kubernetes supports only current and current-2 version

![image](https://user-images.githubusercontent.com/17488415/123376979-ff564d00-d5a8-11eb-8a7a-7d3c7af57f40.png)

upgrade path
![image](https://user-images.githubusercontent.com/17488415/123377000-08dfb500-d5a9-11eb-9205-2e8f4adac23c.png)

Upgrade possibilities
![image](https://user-images.githubusercontent.com/17488415/123377068-1f860c00-d5a9-11eb-83cb-00356b3b00e9.png)

Upgrade plan
1st upgrade master nodes
2nd upgrade worker nodes:

during update master goes down, but pods keep running and services are available.
cluster management is not available. pods, if dead, will not be replaced
