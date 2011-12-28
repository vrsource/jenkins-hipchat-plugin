## HipChat plugin for Jenkins

Started with a fork of the Campfire plugin:

https://github.com/jgp/hudson_campfire_plugin

## Build (ubuntu)
# setup
sudo apt-get install openjdk-6-jdk maven2 # Deps for building
export JAVA_HOME=/usr/lib/jdk/java-6-openjdk

# run the build 
cd <project_dir>
mvn package

# collect the hpi plugin archive
cd target
# jenkins_dir is most likely /var/lib/jenkins
cp jenkins-hipchat-plugin.hpi <jenkins_dir>/plugins

