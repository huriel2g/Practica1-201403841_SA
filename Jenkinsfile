pipeline {
    agent any
    tools { nodejs "node" }

    stages{

      stage('instalando'){
        steps{
            sh 'npm install'
        }
      }

      stage('pruebas'){
        steps{
            sh 'npm test'
        }
      }
  }

}