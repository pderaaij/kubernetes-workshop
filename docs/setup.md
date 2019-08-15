# Workshop setup

In order to run a local kubernetes cluster you have to install [kubectl](#kubectl), [docker](#docker), [virtualbox](#virtualbox) and [minikube](#minikube). Please follow the instructions below to install and verify your installation.

## Kubectl
Kubectl is the command-line tool that lets you execute commands on your kubernetes cluster.

Follow the instructions as found on the [Kubernetes documentation](https://kubernetes.io/docs/tasks/tools/install-kubectl/). Verify the installation has been successfull by running

```
kubectl version
```

At the time of developing this workshop Kubernetes was at version 1.15. All scripts in this workshop should properly function in newer versions as well.

## Docker
Mac and Windows users install Docker Desktop via the [website](https://www.docker.com/products/docker-desktop).

Linux users can simply install Docker Community Edition via their package manager. More information can be found at [Docker Documentation](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

## Virtualbox
Virtualbox is a virtualizer for x86 hardware. We use virtualbox to run our kubernetes cluster.

Download and install Virtualbox via the [Virtualbox website](https://www.virtualbox.org/wiki/Downloads). **NOTE** Install a 6.0 version 

## Minikube
Minikube makes it possible to run a Kubernetes cluster on your local machine. 

Install it by following the instructions as found on the [Getting Starting guide](https://minikube.sigs.k8s.io/docs/start/).

### Mac OS
Mac users are recommended to install minikube via brew. However, the documentations is lacking the step to add the Minikube cask. Before brew install execute:

```
brew cask install minikube
```

After installation please verify the installation by running

```
minikube status
```

If the cluster isn't running, start a cluster by executing

```
minikube start
```