kubectl delete -f cr_example_k8s_instance.yaml
kubectl delete -f ../deploy/service_account.yaml  -n openshift-operators
kubectl delete -f ../deploy/cluster_role.yaml -n openshift-operators
kubectl delete -f ../deploy/cluster_role_binding.yaml -n openshift-operators
kubectl delete -f ../deploy/crds/cis.f5.com_f5bigipctlrs_crd.yaml -n openshift-operators
kubectl delete -f ../deploy/operator.yaml -n openshift-operators
kubectl delete namespace openshift-operators
