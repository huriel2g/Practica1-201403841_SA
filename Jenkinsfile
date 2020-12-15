pipeline {
  agent any

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