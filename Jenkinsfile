pipeline {
  agent any

  stages {
    stage('Clean workspace') {
      steps {
        cleanWs()
      }
    }

    stage('Checkout') {
      steps {
        checkout scmGit(branches: [[name: 'staging']], extensions: [], userRemoteConfigs: [[credentialsId: 'Github-integration', url: 'https://github.com/Net-Pay-Advance-Inc/NPAACH.git']])
      }
    }
