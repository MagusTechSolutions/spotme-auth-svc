// @Library('https://github.com/MagusTechSolutions/mts-jenkins-lib.git') _

library identifier: 'buildJava@master', 
  retriever: modernSCM([
    $class: 'GitSCMSource',
    credentialsId: 'github-repo-token',
    remote: 'https://github.com/MagusTechSolutions/mts-jenkins-lib.git'
  ])

buildJava(
    configFile: 'pipeline.yml',
    jwtCredsId: 'scorepal-rest-jwt-jenkins',
    sonarCredsId: 'Sonarqube'
)