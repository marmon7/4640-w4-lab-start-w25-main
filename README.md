# 4640-w4-lab-start-w25

## Command used to create a new SSH key pair
- ssh-keygen -t ed25519 -f ~/.ssh/<key-name> -C "<comment-to-identify-key>"
- This creates the public key with .pub file extension and a private key no extension
- copy the public key into the cloud-config.yaml file under authorized keys

## General Set Up
- Clone repo to desired directory
- Install AWS CLI and ensure user credentials are authorized: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html#getting-started-install-instructions
- install Terraform: https://developer.hashicorp.com/terraform/install
- run terraform init on root of the repo
- run terraform apply to create the ec2 instance with approriate infastructure.
- SSH into ec2 instance using the dns address or public ip of the generated ec2 instance with the private key: ssh -i ~/.ssh/<private-key> <user>@<host>
