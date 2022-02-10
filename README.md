# Deploy-Container-Service-to-Azure

This template deploys an AKS cluster to Azure

## Initial Setup
1. Fork this project to your Github account.
2. Locally clone your forked version to begin working on the project.

More information on Git and GitHub can be found [here]("https://docs.github.com/en/get-started)

## Variables
Variable are defined in [variables.tf](https://github.com/wallandall/Deploy-Container-Service-to-Azure/blob/main/variables.tf) and their values are stored in [terraform.tfvars](https://github.com/wallandall/Deploy-Container-Service-to-Azure/blob/main/terraform.tfvars)


:warning:
If you are storing sensitive information in terraform.tfvars do not push it to GitHub

* resource_group_name : Name of the resouce group to be created in Azure
* location : Location where your solution will be deployed eg: "West Europe"
* cluster_name : The name of your cluster
* kubernetes_version : The version of Kubernetes. A list of supported versions can be found [here](https://docs.microsoft.com/en-us/azure/aks/supported-kubernetes-versions?tabs=azure-cli)
* system_node_count : Number of Nodes
* node_resource_group : Node resource group