pipeline {
  agent any


  stages{
      stage(build){
        when{
            changeset "**/result/**"
          }

        steps{
          echo 'Compiling result app..'
          dir('worker'){
            sh 'npm install'
          }
        }
      }
      stage(test){
        when{
          changeset "**/result/**"
        }
        steps{
          echo 'Running Unit Tets on result app..'
          dir('result'){
            sh 'npm test'
           }

          }
      }
  }

  post{
    always{
        echo 'Building multibranch pipeline for worker is completed..'
    }
  }
}