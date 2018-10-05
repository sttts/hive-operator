# Opertor for OpenShift Hive

Steps to run the deployment locally

"1." Clone the repository
"1." Make sure you clone the repository in $GOPATH/src/github.com/openshift/
"1." Install [operator-sdk] (https://github.com/operator-framework/operator-sdk)
"1." Make sure minikube is running
"1." run kubectl create -f deploy/crd.yaml
"1." run kubectl create -f deploy/cluster-deployment.yaml
"1." run operator-sdk up local --namespace default --kubeconfig yourconfig
"1." run kubectl create -f deploy/rbac.yaml
"1." run kubectl create -f deploy/cr.yaml

