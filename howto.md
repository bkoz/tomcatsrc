 How to create this repo from scratch

 ```
 mvn archetype:generate -DgroupId=org.koz.app -DartifactId=tomcatsrc -DarchetypeGroupId=org.jboss.weld.archetypes -DarchetypeArtifactId=weld-jsf-servlet-minimal -DinteractiveMode=false
 cd tomcatsrc/
 git remote add origin https://github.com/bkoz/tomcatsrc
 git init .
 git pull origin master
 git add .
 git commit -am "initial code"
 git push
 ```
