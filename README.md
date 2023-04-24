# Linux environment setup

**----- WIP -----**

An Ansible playbook to set up convenient tools in Linux environments for 
different categories, ranging from basic text editor setup to Docker or 
Terraform installations.

## How to use

Run the following command in the root directory:
`ansible-playbook setup.yml [-e tf_version=1.2.6 tg_version=0.43.0]`

Use the `-e` flag ot override the Terraform/Terragrunt version to install if 
running a Terraform installation.