pipeline {
    agent any
    tools { nodejs "node" }

    stages {
		stage ('instalacion de dependencias'){
			steps {
				sh '''
                    npm install
				'''
			}
		}
		stage('Pruebas'){
			steps {
				sh '''
					npm test
				'''
			}
		}
		stage ('Deploy practica'){
			steps {
				sh '''
					npm start
                '''
			}
		}
	}

}