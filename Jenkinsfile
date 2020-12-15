pipeline {
	agent any

    tools{
        nodejs 'NodeJS 8.9.0'
    }
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