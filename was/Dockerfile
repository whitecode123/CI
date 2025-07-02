FROM tomcat:9.0-jdk11-openjdk
COPY ./petclinic_btc/target/petclinic.war /usr/local/tomcat/webapps/ROOT.war
EXPOSE 8080
RUN apt-get update && apt-get install -y default-mysql-client %% rm -rf /var/lib/apt/lists/*
CMD ["catalina.sh", "run"]
