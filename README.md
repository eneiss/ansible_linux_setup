# Linux environment setup

An Ansible playbook to set up convenient tools in Linux environments for 
different categories, ranging from basic text editor setup to Docker or 
Terraform installation.

## How to use

Run the following command in the root directory:
`ansible-playbook setup.yml [-e "var1=value1 var2=value2 ..."] [--tags "tag1 tag2"]`

Use tags to filter which roles to run between the following (omit `--tags` to 
run all roles):
 - aws
 - base
 - docker
 - kubernetes
 - monitoring
 - motd
 - terraform
 - work_env

Use the `-e` flag to override the following settings (variables):
 - `tf_version` and `tg_version`: Terraform/Terragrunt version to install if 
running a Terraform installation.
 - `packages_state`: use `"latest"` to update packages when possible
 - `git_user`: will be reflected in the current user's .gitconfig
 - `git_email`: change this value if you want to use a different email from 
`<git_user>@users.noreply.github.com`