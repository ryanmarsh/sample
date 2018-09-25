How to manage Kubernetes YAML, and deploy with less stress. 

I found HELM https://github.com/helm/helm/tree/master/docs

Helm will help manage all the yaml files from different regions. 

For managing the yaml files we can build a chart to navigate the files and build our deploy, we can even test it with a dryrun built in tool.

Resources https://docs.gitlab.com/ee/install/kubernetes/gitlab_chart.html
https://hk.saowen.com/a/5204da2e0c09e61c001751f5e509104ef7c069e4bc72baf055caa1ed8170701f

Using Helm you can create an umbrella file and set all yaml files under this to deploy using gitlab or jenkins or google cloud. 

The values file can be used to set specific characteristics of each file. Tiller will sort out the application in kubernetes.

Applications of larger scale are easier to deploy and can be tested with Helm, security settings can be set up. 

I believe the permissions can be set so anyone can promote per the Helm docs https://docs.helm.sh/using_helm/ if you use a dev
region or a closed network leaving permissions wide open so devs can promote to it after updating an image should work fine. 

Helm works with gitlabs or jenkins just setting up a git-ci.yaml file. 

For further CI/CD using gitlabs Auto DevOps can streamline the process. 
https://docs.gitlab.com/ee/topics/autodevops/

These two tools combined or seperate should be able to manage the yaml files no matter how numerous. 
