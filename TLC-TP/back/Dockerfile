FROM openjdk:11

RUN apt-get update
RUN apt-get install git

ADD https://api.github.com/repos/StefanLocke/doodlestudent/git/refs/heads/main version.json
RUN git clone https://github.com/StefanLocke/doodlestudent.git

WORKDIR /doodlestudent/api

RUN ./mvnw clean package -DskipTests

WORKDIR /doodlestudent/api/target

ENTRYPOINT [ "java", "-jar", "/doodlestudent/api/target/tlcdemoApp-1.0.0-SNAPSHOT-runner.jar" ]