# tomcatsrc

### Perform an OpenShift source to image build then deploy on Tomcat

#### Build from local source.

```
git clone https://github.com/bkoz/tomcatsrc
cd tomcatsrc
oc login
oc new-project tomcatsrc
oc new-app --image-stream=jboss-webserver30-tomcat7-openshift .
```

After the build and deploy finish, expose the service and visit the route.
```
oc expose service tomcatsrc

firefox http://tomcatsrc-tomcatsrc.ose-apps.haveopen.com/hello
```

#### Build from remote source
```
oc new-app --image-stream=jboss-webserver30-tomcat7-openshift https://github.com/bkoz/tomcatsrc
```
