# Opertor for OpenShift Hive

Steps to run the deployment locally

1) Clone the repository
2) Make sure line number 7 in /pkg/stub/handler.go references the right folder structure
3) Do the same for cmd/hive-operator/main.go line 7 (which references the stub)
4) Go in the deploy directory
5) Make sure minikube is running
6) run kubectl create -f crd.yaml - this creates the CRD
7) Go back to the parent directory
8) run operator-sdk up local --namespace default --kubeconfig yourconfig
9) In another terminal get to the deploy directory
10) run kubectl create -f rbac.yaml
11) run kubectl create -f cr.yaml
12) Go ahead play around

