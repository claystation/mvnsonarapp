# Replicate error

## Steps

Docker build:
`docker build -t sonarapp .`

Run sonarqube:
`docker run sonarapp bash -ce "mvn -f /pom.xml sonar:sonar -Dsonar.host.url=https://somesonarserver.com -Dsonar.login={API_KEY}"`
