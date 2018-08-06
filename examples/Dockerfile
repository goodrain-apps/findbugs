FROM goodrainapps/maven:jdk8-alpine

RUN mkdir /app

COPY . /app/

WORKDIR /app

RUN mvn clean install sonar:sonar -Dsonar.host.url=http://9000.gr26411f.demo.ali-hz.goodrain.net -Dsonar.login=7e9d03f0058be1ec8f8e1febdec3c6d32b6a20b0