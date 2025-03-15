<pre>
<h1> Helm Charts </h1>

[mahsan@r9 tmp]$ helm version
version.BuildInfo{Version:"v3.17.2", GitCommit:"cc0bbbd6d6276b83880042c1ecb34087e84d41eb", GitTreeState:"clean", GoVersion:"go1.23.7"}
[mahsan@r9 tmp]$

[mahsan@r9 tmp]$  helm search hub wordpress
URL                                                     CHART VERSION   APP VERSION             DESCRIPTION
https://artifacthub.io/packages/helm/kube-wordp...      0.1.0           1.1                     this is my wordpress package
https://artifacthub.io/packages/helm/wordpress-...      1.0.2           1.0.0                   A Helm chart for deploying Wordpress+Mariadb st...
https://artifacthub.io/packages/helm/bitnami/wo...      24.1.18         6.7.2                   WordPress is the world's most popular blogging ...
https://artifacthub.io/packages/helm/shubham-wo...      0.1.0           1.16.0                  A Helm chart for Kubernetes
https://artifacthub.io/packages/helm/bitnami-ak...      15.2.13         6.1.0                   WordPress is the world's most popular blogging ...
https://artifacthub.io/packages/helm/camptocamp...      0.6.10          4.8.1                   Web publishing platform for building blogs and ...
https://artifacthub.io/packages/helm/skywordpre...      0.1.0           1.16.0                  A Helm chart for WordPress
https://artifacthub.io/packages/helm/sikademo/w...      2020.11.18                              Example Wordpress Chart (with MySQL)
https://artifacthub.io/packages/helm/devops/wor...      0.12.0          1.16.0                  Wordpress helm chart
https://artifacthub.io/packages/helm/rock8s/wor...      0.12.4          v0.12.4                 An open source content management system
https://artifacthub.io/packages/helm/groundhog2...      0.13.1          6.7.2-apache            A Helm chart for Wordpress on Kubernetes
https://artifacthub.io/packages/helm/sikalabs/w...      0.2.0                                   Simple Wordpress
https://artifacthub.io/packages/helm/riftbit/wo...      12.1.16         5.8.1                   Web publishing platform for building blogs and ...
https://artifacthub.io/packages/helm/schichtel/...      0.7.1           6.6.1                   A Helm chart for WordPress
https://artifacthub.io/packages/helm/homeenterp...      0.5.0           5.9.3-php8.1-apache     Blog server
https://artifacthub.io/packages/helm/mcouliba/w...      0.1.0           1.16.0                  A Helm chart for Kubernetes
https://artifacthub.io/packages/helm/wordpress-...      6.1.1-3.0rc5    master                  Lightweight Wordpress installation with additio...
https://artifacthub.io/packages/helm/wordpress-...      1.0.0           1.1                     This is a package for configuring wordpress and...
https://artifacthub.io/packages/helm/securecode...      4.13.0          4.0                     Insecure & Outdated Wordpress Instance: Never e...
https://artifacthub.io/packages/helm/wordpressm...      1.0.0                                   This is the Helm Chart that creates the Wordpre...
https://artifacthub.io/packages/helm/bitpoke/wo...      0.12.4          v0.12.4                 Bitpoke WordPress Operator Helm Chart
https://artifacthub.io/packages/helm/bitpoke/wo...      0.12.4          v0.12.4                 Helm chart for deploying a WordPress site on Bi...
https://artifacthub.io/packages/helm/kube-wordp...      0.1.0           0.0.1-alpha             Helm Chart for Wordpress installation on MySQL ...
https://artifacthub.io/packages/helm/riotkit-or...      2.1.0-alpha4    v2.1-alpha4             Lightweight Wordpress installation with additio...
https://artifacthub.io/packages/helm/phntom/bin...      0.0.4           0.0.3                   www.binaryvision.co.il static wordpress
https://artifacthub.io/packages/helm/gh-shessel...      2.1.12          6.1.1                   Web publishing platform for building blogs and ...
https://artifacthub.io/packages/helm/rock8s/wor...      6.7.1
https://artifacthub.io/packages/helm/sikalabs/w...      0.1.2
https://artifacthub.io/packages/helm/gh-shessel...      6.3.1           6.3.1                   Web publishing platform for building blogs and ...
https://artifacthub.io/packages/helm/wordpressh...      0.1.0           1.16.0                  A Helm chart for Kubernetes
https://artifacthub.io/packages/helm/wordpress-...      0.1.0           1.1                     this is chart create the wordpress with suitabl...
https://artifacthub.io/packages/helm/wordpress-...      0.0.1                                   Helm Chart for wordpress-gatsby
https://artifacthub.io/packages/helm/bitpoke/bi...      1.8.18          1.8.18                  The Bitpoke App for WordPress provides a versat...
https://artifacthub.io/packages/helm/sonu-wordp...      1.0.0           2                       This is my custom chart to deploy wordpress and...
https://artifacthub.io/packages/helm/uvaise-wor...      0.2.0           1.1.0                   Wordpress for Kubernetes
https://artifacthub.io/packages/helm/wordpress/...      0.2.0           1.1.0                   Wordpress for Kubernetes
https://artifacthub.io/packages/helm/wordpress-...      1.0.0           2                       This is my custom chart to deploy wordpress and...
https://artifacthub.io/packages/helm/bitpoke/stack      0.12.4          v0.12.4                 Your Open-Source, Cloud-Native WordPress Infras...
https://artifacthub.io/packages/helm/securecode...      4.13.0          v3.8.27                 A Helm chart for the WordPress security scanner...
https://artifacthub.io/packages/helm/wordpresss...      1.1.0           5.8.2                   Web publishing platform for building blogs and ...
https://artifacthub.io/packages/helm/viveksahu2...      1.0.0           2                       This is my custom chart to deploy wordpress and...
https://artifacthub.io/packages/helm/six/wordress       0.2.0           1.1.0                   Wordpress for Kubernetes
https://artifacthub.io/packages/helm/jinchi-cha...      0.2.0           1.1.0                   Wordpress for Kubernetes
https://artifacthub.io/packages/helm/projet-dev...      0.1.0           1.16.0                  A Helm chart for wordpress deployed on Azure Ku...
https://artifacthub.io/packages/helm/wordpressm...      0.1.0           1.1
[mahsan@r9 tmp]$

[mahsan@r9 tmp]$ helm repo add stable https://charts.helm.sh/stable
"stable" has been added to your repositories
[mahsan@r9 tmp]$ helm repo list
NAME    URL
stable  https://charts.helm.sh/stable
[mahsan@r9 tmp]$

[mahsan@r9 tmp]$ helm repo list
NAME    URL
stable  https://charts.helm.sh/stable
[mahsan@r9 tmp]$ helm repo add bitnami https://charts.bitnami.com/bitnami
"bitnami" has been added to your repositories
[mahsan@r9 tmp]$ helm repo list
NAME    URL
stable  https://charts.helm.sh/stable
bitnami https://charts.bitnami.com/bitnami
[mahsan@r9 tmp]$

[mahsan@r9 tmp]$  helm search repo stable
NAME                                    CHART VERSION   APP VERSION             DESCRIPTION
stable/acs-engine-autoscaler            2.2.2           2.1.1                   DEPRECATED Scales worker nodes within agent pools
stable/aerospike                        0.3.5           v4.5.0.5                DEPRECATED A Helm chart for Aerospike in Kubern...
stable/airflow                          7.13.3          1.10.12                 DEPRECATED - please use: https://github.com/air...
stable/ambassador                       5.3.2           0.86.1                  DEPRECATED A Helm chart for Datawire Ambassador
stable/anchore-engine                   1.7.0           0.7.3                   Anchore container analysis and policy evaluatio...
stable/apm-server                       2.1.7           7.0.0                   DEPRECATED The server receives data from the El...
stable/ark                              4.2.2           0.10.2                  DEPRECATED A Helm chart for ark
stable/artifactory                      7.3.2           6.1.0                   DEPRECATED Universal Repository Manager support...
stable/artifactory-ha                   0.4.2           6.2.0                   DEPRECATED Universal Repository Manager support...
stable/atlantis                         3.12.4          v0.14.0                 DEPRECATED A Helm chart for Atlantis https://ww...
stable/auditbeat                        1.1.2           6.7.0                   DEPRECATED A lightweight shipper to audit the a...
stable/aws-cluster-autoscaler           0.3.4                                   DEPRECATED Scales worker nodes within autoscali...
stable/aws-iam-authenticator            0.1.5           1.0                     DEPRECATED A Helm chart for aws-iam-authenticator
stable/bitcoind                         1.0.2           0.17.1                  DEPRECATED Bitcoin is an innovative payment net...
stable/bookstack                        1.2.4           0.27.5                  DEPRECATED BookStack is a simple, self-hosted, ...
stable/buildkite                        0.2.4           3                       DEPRECATED Agent for Buildkite
stable/burrow                           1.5.4           0.29.0                  DEPRECATED Burrow is a permissionable smart con...
stable/centrifugo                       3.2.2           2.4.0                   DEPRECATED Centrifugo is a real-time messaging ...
stable/cerebro                          1.9.5           0.9.2                   DEPRECATED A Helm chart for Cerebro - a web adm...
stable/cert-manager                     v0.6.7          v0.6.2                  A Helm chart for cert-manager

[mahsan@r9 tmp]$ helm show chart bitnami/wordpress
annotations:
  category: CMS
  images: |
    - name: apache-exporter
      image: docker.io/bitnami/apache-exporter:1.0.9-debian-12-r17
    - name: os-shell
      image: docker.io/bitnami/os-shell:12-debian-12-r39
    - name: wordpress
      image: docker.io/bitnami/wordpress:6.7.2-debian-12-r8
  licenses: Apache-2.0
apiVersion: v2
appVersion: 6.7.2
dependencies:
- condition: memcached.enabled
  name: memcached
  repository: oci://registry-1.docker.io/bitnamicharts
  version: 7.x.x
- condition: mariadb.enabled
  name: mariadb
  repository: oci://registry-1.docker.io/bitnamicharts
  version: 20.x.x
- name: common
  repository: oci://registry-1.docker.io/bitnamicharts
  tags:
  - bitnami-common
  version: 2.x.x
description: WordPress is the world's most popular blogging and content management
  platform. Powerful yet simple, everyone from students to global corporations use
  it to build beautiful, functional websites.
home: https://bitnami.com
icon: https://dyltqmyl993wv.cloudfront.net/assets/stacks/wordpress/img/wordpress-stack-220x234.png
keywords:
- application
- blog
- cms
- http
- php
- web
- wordpress
maintainers:
- name: Broadcom, Inc. All Rights Reserved.
  url: https://github.com/bitnami/charts
name: wordpress
sources:
- https://github.com/bitnami/charts/tree/main/bitnami/wordpress
version: 24.1.18


[mahsan@r9 tmp]$ helm install wordpress bitnami/wordpress
NAME: wordpress
LAST DEPLOYED: Sat Mar 15 15:08:38 2025
NAMESPACE: helm
STATUS: deployed
REVISION: 1
TEST SUITE: None
NOTES:
CHART NAME: wordpress
CHART VERSION: 24.1.18
APP VERSION: 6.7.2

Did you know there are enterprise versions of the Bitnami catalog? For enhanced secure software supply chain features, unlimited pulls from Docker, LTS support, or application customization, see Bitnami Premium or Tanzu Application Catalog. See https://www.arrow.com/globalecs/na/vendors/bitnami for more information.

** Please be patient while the chart is being deployed **

Your WordPress site can be accessed through the following DNS name from within your cluster:

    wordpress.helm.svc.cluster.local (port 80)

To access your WordPress site from outside the cluster follow the steps below:

1. Get the WordPress URL by running these commands:

  NOTE: It may take a few minutes for the LoadBalancer IP to be available.
        Watch the status with: 'kubectl get svc --namespace helm -w wordpress'

   export SERVICE_IP=$(kubectl get svc --namespace helm wordpress --template "{{ range (index .status.loadBalancer.ingress 0) }}{{ . }}{{ end }}")
   echo "WordPress URL: http://$SERVICE_IP/"
   echo "WordPress Admin URL: http://$SERVICE_IP/admin"

2. Open a browser and access WordPress using the obtained URL.

3. Login with the following credentials below to see your blog:

  echo Username: user
  echo Password: $(kubectl get secret --namespace helm wordpress -o jsonpath="{.data.wordpress-password}" | base64 -d)

WARNING: There are "resources" sections in the chart not set. Using "resourcesPreset" is not recommended for production. For production installations, please set the following values according to your workload needs:
  - resources
+info https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
[mahsan@r9 tmp]$

[mahsan@r9 tmp]$ oc get all
Warning: apps.openshift.io/v1 DeploymentConfig is deprecated in v4.14+, unavailable in v4.10000+
NAME                            READY   STATUS    RESTARTS   AGE
pod/wordpress-b678d4dc8-2x5fx   0/1     Running   0          75s
pod/wordpress-mariadb-0         0/1     Running   0          75s

NAME                                 TYPE           CLUSTER-IP    EXTERNAL-IP   PORT(S)                      AGE
service/wordpress                    LoadBalancer   10.217.5.17   <pending>     80:30333/TCP,443:31837/TCP   75s
service/wordpress-mariadb            ClusterIP      10.217.4.88   <none>        3306/TCP                     75s
service/wordpress-mariadb-headless   ClusterIP      None          <none>        3306/TCP                     75s

NAME                        READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/wordpress   0/1     1            0           75s

NAME                                  DESIRED   CURRENT   READY   AGE
replicaset.apps/wordpress-b678d4dc8   1         1         0       75s

NAME                                 READY   AGE
statefulset.apps/wordpress-mariadb   0/1     75s
[mahsan@r9 tmp]$

[mahsan@r9 tmp]$ helm list
NAME            NAMESPACE       REVISION        UPDATED                                 STATUS          CHART                   APP VERSION
wordpress       helm            1               2025-03-15 15:08:38.930903654 -0700 PDT deployed        wordpress-24.1.18       6.7.2
[mahsan@r9 tmp]$

[mahsan@r9 tmp]$ helm status wordpress
NAME: wordpress
LAST DEPLOYED: Sat Mar 15 15:08:38 2025
NAMESPACE: helm
STATUS: deployed
REVISION: 1
TEST SUITE: None
NOTES:
CHART NAME: wordpress
CHART VERSION: 24.1.18
APP VERSION: 6.7.2

Did you know there are enterprise versions of the Bitnami catalog? For enhanced secure software supply chain features, unlimited pulls from Docker, LTS support, or application customization, see Bitnami Premium or Tanzu Application Catalog. See https://www.arrow.com/globalecs/na/vendors/bitnami for more information.

** Please be patient while the chart is being deployed **

Your WordPress site can be accessed through the following DNS name from within your cluster:

    wordpress.helm.svc.cluster.local (port 80)

To access your WordPress site from outside the cluster follow the steps below:

1. Get the WordPress URL by running these commands:

  NOTE: It may take a few minutes for the LoadBalancer IP to be available.
        Watch the status with: 'kubectl get svc --namespace helm -w wordpress'

   export SERVICE_IP=$(kubectl get svc --namespace helm wordpress --template "{{ range (index .status.loadBalancer.ingress 0) }}{{ . }}{{ end }}")
   echo "WordPress URL: http://$SERVICE_IP/"
   echo "WordPress Admin URL: http://$SERVICE_IP/admin"

2. Open a browser and access WordPress using the obtained URL.

3. Login with the following credentials below to see your blog:

  echo Username: user
  echo Password: $(kubectl get secret --namespace helm wordpress -o jsonpath="{.data.wordpress-password}" | base64 -d)

WARNING: There are "resources" sections in the chart not set. Using "resourcesPreset" is not recommended for production. For production installations, please set the following values according to your workload needs:
  - resources

[mahsan@r9 tmp]$ oc  get secret --namespace helm wordpress -o jsonpath="{.data.wordpress-password}" | base64 -
WWtsV09XSnhRbWxWV1E9PQ==

[mahsan@r9 tmp]$ oc get svc
NAME                         TYPE           CLUSTER-IP    EXTERNAL-IP   PORT(S)                      AGE
wordpress                    LoadBalancer   10.217.5.17   <pending>     80:30333/TCP,443:31837/TCP   5m
wordpress-mariadb            ClusterIP      10.217.4.88   <none>        3306/TCP                     5m
wordpress-mariadb-headless   ClusterIP      None          <none>        3306/TCP                     5m
[mahsan@r9 tmp]$ oc expose svc wordpress
route.route.openshift.io/wordpress exposed
[mahsan@r9 tmp]$ oc get routes.route.openshift.io
NAME        HOST/PORT                         PATH   SERVICES    PORT   TERMINATION   WILDCARD
wordpress   wordpress-helm.apps-crc.testing          wordpress   http                 None

[mahsan@r9 tmp]$ helm list
NAME            NAMESPACE       REVISION        UPDATED                                 STATUS          CHART                   APP VERSION
wordpress       helm            1               2025-03-15 15:08:38.930903654 -0700 PDT deployed        wordpress-24.1.18       6.7.2
[mahsan@r9 tmp]$ helm uninstall wordpress
release "wordpress" uninstalled
[mahsan@r9 tmp]$ helm list
NAME    NAMESPACE       REVISION        UPDATED STATUS  CHART   APP VERSION
[mahsan@r9 tmp]$







</pre>

