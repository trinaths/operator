oc project openshift-operators
oc apply -f ../deploy/service_account.yaml -n openshift-operators
oc apply -f ../deploy/cluster_role.yaml -n openshift-operators
oc apply -f ../deploy/cluster_role_binding.yaml -n openshift-operators
oc apply -f ../deploy/crds/cis.f5.com_f5bigipctlrs_crd.yaml -n openshift-operators
oc apply -f ../deploy/operator.yaml -n openshift-operators
oc apply -f cr_example_ocp_instance.yaml 
