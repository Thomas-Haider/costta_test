pipeline {
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/renestadler/costta'
      }
    }
    stage('Install dependencies') {
      steps {
        bat 'npm install'
      }
    }
    stage('Building') {
      steps {
        sh 'npm run build'
      }
    }
    stage('Starting') {
      steps {
        sh 'npm start'
      }
    }
  }
}