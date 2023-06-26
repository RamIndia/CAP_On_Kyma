# Prerequisites for Deploying CAP applications on Kyma
 - For Windows, you'll need Chocolatey. This is a package manager that will speed up and ease installation of the tools in this tutorial. See how to install Chocolatey in [Setup/Install](https://docs.chocolatey.org/en-us/choco/setup).
 - For Mac OSX, you need brew. You can install latest version of [brew](https://brew.sh/).

## Verify your @sap/cds and @sap/cds-dk versions

Make sure you're using the latest CAP tooling version.

1. `npm install --global @sap/cds-dk` to install globally the latest `@sap/cds-dk` version.

1. `npm install` to install your local package.

2. `cds version` to double check that the globally installed `@sap/cds-dk` version and your locally installed `@sap/cds` version match.

Note: Make sure cds version is > 7.0!

## Install kubectl

### macOS
1. To install kubectl, run the following command:
    
    ```bash
    brew install kubectl
    ```
    
2. Check if the installation is successful:
    
    ```bash
    kubectl version --client
    ```
    
    You should see a version number.
    
### Windows
You can install kubectl using chocolatey.
1. To install kubectl, run the following command:
    
    ```bash
    choco install kubernetes-cli
    ```
    
2. Check if the installation is successful:
    
    ```bash
    kubectl version --client
    ```

### Linux
Follow the instructions for your preferred way of installing kubectl at [Install and Set Up kubectl on Linux](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/).

## Install helm

There's a multitude of options to install helm. You can see the full list at [Installing Helm](https://helm.sh/docs/intro/install/). We have also listed some options:

### macOS
1. To install helm, run the following command:
    
    ```bash
    brew install helm
    ```
    
2. Check if the installation is successful:
    
    ```bash
    helm version
    ```
    
### Windows
You can install helm using chocolatey.
1. To install helm run the following command:
    
    ```bash
    choco install kubernetes-helm
    ```
2. Check if the installation is successful:
   
    ```bash
    helm version
    ```

## Install Paketo (pack)
Pack lets you build container images, which are collaboratively maintained making it easier to maintain and update.
Install the [pack CLI](https://buildpacks.io/docs/tools/pack/#install).

### macOS
You can install pack using brew with the command:

```bash
brew install buildpacks/tap/pack
```
    
### Windows
You can install pack using chocolatey with the command:

 ```bash
 choco install pack --version=0.29.0
 ```
    
### Linux
Follow the instructions to install the [pack CLI](https://buildpacks.io/docs/tools/pack/#install).


## Install Docker Desktop

Kyma runs on containers. Hence, for this tutorial, you'll need an application that enables you to manage (build, push, pull, and run) container images on your desktop and a docker-compatible command line interface. In this session we will use Docker Desktop.
### macOS:
 Download the installer from [Install Docker Desktop on Mac](https://docs.docker.com/desktop/mac/install/) and follow the instructions to install and set up Docker Desktop.

### Windows:
 Download the installer from [Install Docker Desktop on Windows](https://docs.docker.com/desktop/windows/install/) and follow the instructions to install and set up Docker Desktop.




