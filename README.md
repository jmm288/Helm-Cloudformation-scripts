# InCharge Energy Tasks
## Task 1: Create a Helm Chart 
### Should contain:
* 2 deployments (API, Background) each deployment uses one image, but different launch parameters.
* Configmap for config file.
* Ingress sends requests to pods with API parameters only.
* Cronjob which is executed once a day (same image, cronjob parameter)

Solution:
* HelmCharts/

### Comments:
* I put something together with what was requested but couldn't exactly figure out the way you wanted it with the time I had. I think there was an easier, expected way to create the deployments from one deployment file and then dynamically pass the launch parameters, but I wasn't sure how to do it.

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

### Comments: 
* I wasn't exactly sure what to do with the /23 /18, I understood they likely had something to do with the slash notation of the expected range of IP addresses of each subnet? But I wasn't sure where to put the information, Networking is not my expertise.
