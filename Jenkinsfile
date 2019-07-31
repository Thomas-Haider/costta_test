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
        bat 'npm run build'
      }
    }
    stage('Starting') {
      steps {
        bat 'npm start'
      }
    }
  }
}