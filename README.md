# gcpbash
Bash scripts and Google Cloud SDK commands for building and architecting solutions for IAM and IaC. 
Each file is simple and straight forward for creating scenarios for:

 - IAM policies with multiple admins for a project in an organization. (CLI or SDK) run after initiating project or through web console. 

  - Scripts for deploying VPC peering among two VPC's and checking if the connection already exist. 

   - Conditional bash script for restricting admin access with conditional expression for (business hours access only) (Bash)
   
When automating IAM on Google Cloud you can set the conditional access for many different levels in the project resources by interacting with the API. For instance you may want to give one developer ```read``` access to a bucket while access to ```create``` buckets is disabled. 

Conditional expressions can be authored to act as blueprints for continuous deployments. 

[Google Cloud Overview of IAM Conditions.](https://cloud.google.com/iam/docs/conditions-overview)  

Consider using templates for deploying resources at a larger scale which is best suited when using an IaC solution such as [Terraform](https://registry.terraform.io/modules/terraform-google-modules/project-factory/google/latest). 

[Refer to the Project Factory Module from the Terraform Registry.](https://registry.terraform.io/modules/terraform-google-modules/project-factory/google/latest) 
