# Step 1: Use Tomcat base image
FROM tomcat:9-jdk11

# Step 2: Remove default Tomcat apps
RUN rm -rf /usr/local/tomcat/webapps/*

# Step 3: Copy WAR file into Tomcat
COPY target/char-webapp-1.0-SNAPSHOT.war /usr/local/tomcat/webapps/ROOT.war

# Step 4: Expose Tomcat port
EXPOSE 8080

# Step 5: Start Tomcat
CMD ["catalina.sh", "run"]

