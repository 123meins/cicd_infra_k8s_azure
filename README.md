## cicd_infra_k8s_azure
cicd projekt with terraform, azure devops and k8s

## Getting started

#
pipline is deactivated, no infrastructure is running

# install azure cli
```
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

# login into azure
```
az login
```

# create service account for your to create azure k8s cluster
```
az ad sp create-for-rbac --role="Contributor" --scopes="/subscrioptions/[subscriptionID]"
```
# create connection to azure devops
dev.azure.com
project settings
service connections
new Azure Resource Manager

# install terraform plugins
marketplace
install DevLabs Charles Zipp

# create pipline
github
starter pipeline

# get credentials to k8s cluster to use kubectl
az aks get-credentials --name k8stest_dev --resource-group kubernetes_dev

# to do
add code analysis tools (sonarqube)