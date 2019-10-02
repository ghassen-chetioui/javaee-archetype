FROM jboss/wildfly
RUN /opt/jboss/wildfly/bin/add-user.sh admin admin#007 --silent
ADD target/${artifactId}.war ${JBOSS_HOME}/standalone/deployments/
CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]