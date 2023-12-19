pipeline {
  agent any

  stages {
    stage('Clean workspace') {
      steps {
        cleanWs()
      }
    }

    stage('Checkout-1') {
      steps {
        checkout scmGit(branches: [[name: 'staging']], extensions: [], userRemoteConfigs: [[credentialsId: 'Github-integration', url: 'https://github.com/Net-Pay-Advance-Inc/NPAACH.git']])
      }
    }
