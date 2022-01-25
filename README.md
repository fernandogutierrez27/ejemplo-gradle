# Getting Started

## Windows

### Compile Code
### Test Code
### Jar Code
* ./gradlew.bat clean build

### Run Jar
* Local:      ./gradlew.bat bootRun

### Testing Application
* Abrir navegador: http://localhost:8082/rest/mscovid/test?msg=testing

## Linux

### Compile Code
### Test Code
### Jar Code
* ./gradlew clean build

### Run Jar
* Local:      ./gradlew bootRun

### Testing Application
* curl -X GET 'http://localhost:8082/rest/mscovid/test?msg=testing'

# Using Docker to test this app.
⚠️ **Is mandatory to use Powershell in Windows**
## Docker in Windows
```bash
### Compile Code
### Test Code
### Jar Code
docker run -it --rm -v ${pwd}:/code --workdir /code gradle gradle clean build

### Run Jar
docker run -it --rm -p 8082:8082  -v ${pwd}:/code --workdir /code gradle gradle bootRun
```
## Docker in Linux
```bash
### Compile Code
### Test Code
### Jar Code
docker run -it --rm -v $(pwd):/code --workdir /code gradle gradle clean build

### Run Jar
docker run -it --rm -p 8082:8082  -v $(pwd):/code --workdir /code gradle gradle bootRun
```