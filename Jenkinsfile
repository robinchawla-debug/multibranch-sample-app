@Library("shared-library") _
pipeline {
  agent {label 'linux'}
  options {
    buildDiscarder(logRotator(artifactDaysToKeepStr: '',artifactNumToKeepStr:'5',daysToKeepStr:'',numToKeepStr: '5'))
    disableConcurrentBuilds()
  }
  stages {
    stage('Hello') {
      steps {
        helloWorld(name:"robin",dayOfWeek:"thursday");
      }
    }
  }
}
