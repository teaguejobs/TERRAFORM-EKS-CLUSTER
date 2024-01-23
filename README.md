#MANAGE EKS WITH TERRAFORM

# PREREQUISITES

1. Install Terraform CLI

2. Install AWS CLI

3. have the kubernentes.tf file

4. Have the resource_nginx.tf file

5. Have the service_eks_nginx.tf file

6. Have the outputs_eks.tf file


OBJECTIVES

1. Create demo-terraform-manage-eks directory and cd into it

2. Download the kubernetes_eks.tf file and view the file and Rename the file

`wget -0 kubernetes.tf https://raw.githubusercontent.com/teaguejobs/content-terraform-2021/main/kubernetes_eks.tf`

3. Apply the configuration and verify the eks cluster is running 

`terraform init`

`terraform apply`

NOTE: Make sure to use thesame statefile for the previous project https://github.com/teaguejobs/Terraform-And-Kubernetes.Else you will need to provision a new cluster from ground up.

4. Download the resource_nginx.tf file

`wget https://raw.githubusercontent.com/teaguejobs/content-terraform-2021/main/resource_nginx.tf`

5. View the file and apply the configuration to schedule nginx deployment

`terraform apply`

6. Verify the nginx deployment is running

`kubectl get deployment`

7. Download the service_eks_nginx.tf file 

`wget https://raw.githubusercontent.com/teaguejobs/content-terraform-2021/main/service_eks_nginx.tf`


8. Download the outputs_eks.tf file


`wget https://raw.githubusercontent.com/teaguejobs/content-terraform-2021/main/outputs_eks_nginx.tf`

9. View the file and apply the configuration to schedule load balancer deployment

`terraform apply`

10. Verify load balancer deployment is running

11. Scale the deployment from 2-4 on our resource_nginx.tf file
