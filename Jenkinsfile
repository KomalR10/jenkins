pipeline {
stages {
stage(checkout) {
  git'https://github.com/KomalR10/jenkins.git'
}
stage(build) {
bat 'mvn clean package'
withSonarQubeEnv('Sonar') {
    mvn sonar:sonar
}
}
}
}
