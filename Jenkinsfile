properties([
          [$class: 'GithubProjectProperty',
         displayName: '',
         projectUrlStr: 'https://github.com/Avengers-marvel/Defenders.git'],
         pipelineTriggers([
         upstream(
          threshold: 'SUCCESS',
           upstreamProjects: 'https://github.com/Avengers-marvel/Inhumans.git'    )])
  ])

pipeline {
  agent any 

  stages {
      stage('Build') {
          steps {
              echo " This is Builld Staage"
          }
      }
      stage('Test'){
          steps {
              echo "This is a Test Stagee"
          }
      }
      stage('Deploy') {
          steps {
              echo "This is a Deploy Stage here"
          }
      }
  }
}
