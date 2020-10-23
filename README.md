# terraform-commands
This repo highlights the common commands in Terraform

### terraform init 
- Used to initialize a working directory containing Terraform configuration files. **This is the first command that should be run** after writing a new Terraform configuration or cloning an existing one from version control. It is safe to run this command multiple times. See [Command: init](https://www.terraform.io/docs/commands/init.html) for more info


### terraform plan

- (Optional) The terraform plan command is used to create an execution plan - This is basically a dry-run of the code. Although, this is optional, it is recommended to get an idea of the changes that will be performed by the code. This command is a convenient way to check whether the execution plan for a set of changes matches your expectations without making any changes to real resources or to the state. See [Command: plan](https://www.terraform.io/docs/commands/plan.html) for more info


### terraform apply
- Run this command to actually run the code. By default, apply scans the current directory for the configuration and applies the changes appropriately. However, a path to another configuration or an execution plan can be provided. Explicit execution plan files can be used to split plan and apply into separate steps within [automation systems](https://learn.hashicorp.com/terraform/development/running-terraform-in-automation). See [Command: apply](https://www.terraform.io/docs/commands/apply.html) for more info


### terraform destroy
- This command destroy/deletes/removes the resources that have been created by Terraform. This will ask for confirmation before destroying. See [Command: destroy](https://www.terraform.io/docs/commands/destroy.html) for more info
