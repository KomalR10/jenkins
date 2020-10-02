pipeline {

stages {

stage(checkout) {

  git: 
}

stage(build) {

bat 'mvn clean package'
withSonarQubeEnv('Sonar') {
    mvn sonar:sonar
}
