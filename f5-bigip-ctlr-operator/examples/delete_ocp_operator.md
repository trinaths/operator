#oc delete -f cr_example_ocp_instance.yaml
oc delete -f ../deploy/service_account.yaml  -n openshift-operators
oc delete -f ../deploy/cluster_role.yaml -n openshift-operators
oc delete -f ../deploy/cluster_role_binding.yaml -n openshift-operators
oc delete -f ../deploy/crds/cis.f5.com_f5bigipctlrs_crd.yaml -n openshift-operators
oc delete -f ../deploy/operator.yaml -n openshift-operators
