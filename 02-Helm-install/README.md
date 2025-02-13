# Helm Install

## Step-01: Introduction
  * We will use the following commands as part of this demo
  * helm repo list
  * helm repo add
  * helm repo update
  * helm search repo
  * helm install
  * helm list
  * helm uninstall

## Step-02: List, Add and Search Helm Repository
   
   [Bitnami Applications Packaged using Helm ](https://bitnami.com/stacks/helm)

   [Search for Helm charts at Artifacthub.io](https://artifacthub.io/)

    # List Helm Repositories
    helm repo list

    # Add Helm Repository
    helm repo add <DESIRED-NAME> <HELM-REPO-URL>
    helm repo add mybitnami https://charts.bitnami.com/bitnami

    # List Helm Repositories
    helm repo list

    # Search Helm Repository
    helm search repo <KEY-WORD>
    helm search repo nginx
    helm search repo apache
    helm search repo wildfly

## Step-03: Install Helm Chart

  * Installs the Helm Chart
        # Update Helm Repo
        helm repo update  # Make sure we get the latest list of charts

        # Install Helm Chart
        helm install <RELEASE-NAME> <repo_name_in_your_local_desktop/chart_name>
        helm install mynginx mybitnami/nginx

## Step-04: List Helm Releases
  * This command lists all of the releases for a specified namespace

        # List Helm Releases (Default Table Output)
        helm list 
        helm ls

        # List Helm Releases (YAML Output)
        helm list --output=yaml
    
        # List Helm Releases (JSON Output)
        helm list --output=json
    
        # List Helm Releases with namespace flag
        helm list --namespace=default
        helm list -n default
