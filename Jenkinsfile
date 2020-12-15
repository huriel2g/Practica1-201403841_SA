pipeline {
	agent any
	stages {
		stage ('instalacion de dependencias'){
			steps {
				sh '''
					npm install
				'''
			}
		}
		stage('Mi Build'){
			steps {
				sh '''
					cd PracticaSA/
					npm test
				'''
			}
		}
		stage ('Deploy practica'){
			steps {
				sh '''
					cd PracticaSA/
					npm start
                '''
			}
		}
	}
}