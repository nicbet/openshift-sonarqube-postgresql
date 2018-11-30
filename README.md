# openshift-sonarqube-postgresql
Template for running SonarQube using Postgresql with Persistent Volumes in OpenShift

## Adding the Template to OpenShift
Create the template in your OpenShift cluster like this:

```
oc login -u system:admin

oc project openshift

oc create -f sonarqube-postgresql-template.json
```

## Removing the Template
In case your want to upload a new version of it:

```
oc delete template/sonarqube -n openshift
```