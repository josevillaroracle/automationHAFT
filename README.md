# automationHAFT
OCI01
This set Ansible set, will create a full HA environment with AD fault tolerance, with a VCN with all the associated subnets, Route Tables, IGW, DRG, Security Lists with the Security Rules, Load Balancer Tier, a Web App Tier cluster instances and configure them, File Storages replicated with Rsync and Databases with DG.
For that we will:
Create a compartment that will host a simple VCN with a simple subnet, an IGW and a single instance and install in it ansyble and python 3.6. instructions in the aditional document.
In this case we are setting up minimal elements because of our target architecture and our demo environment characteristics.
Steps:
  1. Create a container: DevOPSHA
  2. Create User token in identity and save it secured.
  3. Import the ansible project from here with GIT clone
  4. Copy own id for tenancy, compartment, user plus token in ansible config file in the instance acting as ansible machine in OCI.
     Replace in vardef.yaml the variables with your own for the ID
  5. Run Playbook.yaml
