## Udacity DevOps
This repo is/will be structured by project. All project content will be in the relevant project folder except for common variables/scripts which will be stored in the shared_varibales folder.
Each folder will contain a seperate README file to provide info for that folder

### Dependencies
#### 1. AWS account
You would require to have an AWS account to be able to build cloud infrastructure.

#### 2. S3 Folder
I've used my own folder, so if you want to recreate some scripts you will need to create your own folder and add it as a varibale.

### How to run the create/update scripts?
You can run the supporting material in two easy steps:
```bash
# Ensure that the AWS CLI is configured before runniing the command below
# Create the network infrastructure
# Check the region in the create.sh file
./create.sh myFirstStack network.yml network-parameters.json
# Create servers
# Change the AMI ID and key-pair name in the servers.yml
# Check the region in the update.sh file
./update.sh mySecStack servers.yml server-parameters.json
```