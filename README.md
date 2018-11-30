Steps to run the deployment locally

1) Clone the repository
2) Make sure you clone the repository in $GOPATH/src/github.com/openshift/
3) Install [operator-sdk](https://github.com/operator-framework/operator-sdk)
4) Make sure minikube is running
5) Create the resources in the order given in the manifest folder using the following instruction kubectl create -f manifest/<filename>
6) run operator-sdk up local --namespace default --kubeconfig <your_config>
7) kubectl create -f deploy/crds/hive_v1alpha1_hive_cr.yaml

