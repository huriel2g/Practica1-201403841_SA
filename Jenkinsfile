pipeline {
    agent any
    tools { nodejs "node" }

    stages {
		stage ('instalacion de dependencias'){
			steps {
				sh '''
                    cd PracticaSA/
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