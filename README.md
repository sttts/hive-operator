# Opertor for OpenShift Hive

Steps to run the deployment locally

1. Clone the repository
2. Make sure you clone the repository in $GOPATH/src/github.com/openshift/
3. Install [operator-sdk](https://github.com/operator-framework/operator-sdk)
4. Make sure minikube is running
5. run kubectl create -f deploy/crd.yaml
6. run kubectl create -f deploy/cluster-deployment.yaml
7. run operator-sdk up local --namespace default --kubeconfig yourconfig
8. run kubectl create -f deploy/rbac.yaml
9. run kubectl create -f deploy/cr.yaml

