FROM openjdk:8
# Add a volume pointing to /tmp
VOLUME /tmp
# Make port 8080 available to the world outside this container
EXPOSE 8080

# The application's jar file
#ARG JAR_FILE=target/ms_GestionEnseignant:0.0.1-SNAPSHOT.jar

ADD target/ms_GestionEnseignant-0.0.1-SNAPSHOT.jar enseignant.jar

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom", "-jar", "/enseignant.jar"]

