kubectl create namespace openshift-operators
kubectl apply -f ../deploy/service_account.yaml -n openshift-operators
kubectl apply -f ../deploy/cluster_role.yaml -n openshift-operators
kubectl apply -f ../deploy/cluster_role_binding.yaml -n openshift-operators
kubectl apply -f ../deploy/crds/cis.f5.com_f5bigipctlrs_crd.yaml -n openshift-operators
kubectl apply -f ../deploy/operator.yaml -n openshift-operators
kubectl apply -f cr_example_k8s_instance.yaml 
