# helm-github

This is a helm plugin that installs raw helm charts from github.

# Installation
  * `helm plugin install --version master https://github.com/sagansystems/helm-github.git`
  * `helm github --help`

![image](https://user-images.githubusercontent.com/52489/33590100-fa79e052-d931-11e7-9879-b0fd7db7d09a.png)

# Updates

### Automatically
  * `helm github --update`

### Manually
  * `cd $HELM_HOME/plugins/`
  * `git pull`
 
# Usage
  * `helm github install --repo git@github.com:kubernetes/charts.git --path stable/external-dns/`
  * `helm github install --repo git@github.com:coreos/alb-ingress-controller.git --ref 6d64984 --path alb-ingress-controller-helm`
  * `helm github install --repo git@github.com:coreos/alb-ingress-controller.git --ref master --path alb-ingress-controller-helm --namespace kube-system --name alb-ingress-ctlr-1 -f alb-ingress-controller/values.yml --version 0.0.6`
