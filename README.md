# Linux environment setup

**----- WIP -----**

An Ansible playbook to set up convenient tools in Linux environments for 
different categories, ranging from basic text editor setup to Docker or 
Terraform installation.

## How to use

Run the following command in the root directory:
`ansible-playbook setup.yml [-e "var1=value1 var2=value2 ..."]`

Use the `-e` flag to override the following settings (variables):
 - `tf_version` and `tg_version`: Terraform/Terragrunt version to install if 
running a Terraform installation.
 - `packages_state`: use `"latest"` to update packages when possible