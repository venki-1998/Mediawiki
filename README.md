# Mediawiki

# What is MediaWiki?
MediaWiki is free and open-source wiki software. Originally developed by Magnus Manske and improved by Lee Daniel Crocker, it runs on many websites, including Wikipedia, Wiktionary and Wikimedia Commons. It is written in the PHP programming language and stores the contents into a database. Like WordPress, which is based on a similar licensing and architecture, it has become the dominant software in its category.

# Helm Charts files
mediawiki-chart - For installing and configuring Mediawiki on a Centos7 container.
mediawiki-mariadb-chart - For installing and configuring Mariadb for handling Mediawiki database.

Install the Helm chart using command:

helm install mediawiki ./mediawiki-chart -n <NAMESPACE>
helm install database ./mediawiki-mariadb-chart -n <NAMESPACE>

# Kubernetes
The kubernetes objects are defined in following files: deployment.yaml,ingress.yaml,networkpolicy.yaml,pvc.yaml,service.yaml,secrets.yaml,Chart.yaml,values.yaml

