# k8s-local-setup
Setting up a local Kubernetes cluster.

### 1. Install Kubectl

Kubectl is a command-line tool for interacting with Kubernetes clusters. 
It can be used to deploy, manage, and inspect the state of applications running on a Kubernetes cluster.

If you are on macOS, and using homebrew you can simply do:
```shell
brew install kubectl
```

For up-to-date information on how to install `kubectl` on any other OS, please refer to the [official installation guide](https://kubernetes.io/docs/tasks/tools/#kubectl).

To check the installation, simply run:
```shell
kubectl version
```

This command should display both `client version` and `server version` details. Something like this:
```shell
Client Version: version.Info{Major:"1", Minor:"25", GitVersion:"v1.25.2", GitCommit:"5835544ca568b757a8ecae5c153f317e5736700e", GitTreeState:"clean", BuildDate:"2022-09-21T14:33:49Z", GoVersion:"go1.19.1", Compiler:"gc", Platform:"darwin/amd64"}
Kustomize Version: v4.5.7
Server Version: version.Info{Major:"1", Minor:"23", GitVersion:"v1.23.14-gke.401", GitCommit:"aafb848fb0f7414f744ec2835516352f9f2620bf", GitTreeState:"clean", BuildDate:"2022-11-28T16:13:06Z", GoVersion:"go1.17.13b7", Compiler:"gc", Platform:"linux/amd64"}
WARNING: version difference between client (1.25) and server (1.23) exceeds the supported minor version skew of +/-1
```