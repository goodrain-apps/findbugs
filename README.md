# README.md

## 部署 Docker run

```bash
docker run --name postgresql -p 5432:5432 -e POSTGRES_USER=sonar -e POSTGRES_PASSWORD=sonar -e POSTGRE_DB=sonar -d postgres:10.4
# 依赖postgresql
docker run --name sonarqube -e SONARQUBE_JDBC_URL=jdbc:postgresql://127.0.0.1:5432/sonar -p 9000:9000 -d sonarqube:7.1
```

参考 [docker-sonarqube](https://github.com/SonarSource/docker-sonarqube/blob/master/recipes.md)

## Usage

具体使用可以参考example