# lenovo-poc
you will find the CRD ( manifests) used to deploy SNO / Spoke clusters using ACM + ZTP for the following lenovo servers:
- ThinkEdge SE450 
- ThinkSystem SR630 V2.

below is the structure of the directories: 

   clusters-app.yaml
   prereq
      prereq-lenovo
      prereq-lenovo-1
   ztp-policy-generator
      bellerica-lenovo-2.yaml
      bellerica-lenovo.yaml
      kustomization.yaml

- clusters-app.yaml is the manifest you to deploy an argocd app to automate the SNO/Spoke cluster deployment.
- prereq directory has the files used to create the secret and the namespace that will be used by the BMH object ( baremetal Host)
- ztp-policy-generator directory has the siteconfig CRD used. Kustomization is used to deploy the spoke clusters.


