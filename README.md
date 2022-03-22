# InCharge Energy Tasks
## Task 1: Create a Helm Chart 
### Should contain:
* 2 deployments (API, Background) each deployment uses one image, but different launch parameters.
* Configmap for config file.
* Ingress sends requests to pods with API parameters only.
* Cronjob which is executed once a day (same image, cronjob parameter)

Solution:
* HelmCharts/Chart.yaml

## Task 2: Create a CloudFormation Template
### Should contain:
* 3 public subnets /23
* 3 private subnets /18 
	*  With 2 subnets in each Availability Zone, also an ipv6 network in each subnet.
* NAT Gateway (for private subnets)
* Egress only internet gateway (for private subnets)
* Internet Gateway (for public subnets)

Solution:
* CloudformationTemplates/Template.yaml
