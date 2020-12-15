pipeline {
	agent any

	stages {
		stage ('instalacion de dependencias'){
			steps {
				sh '''
					cd Practica1-201403841_SA
					npm install
				'''
			}
		}
		stage('Mi Build'){
			steps {
				sh '''
					cd Practica1-201403841_SA
					npm test
				'''
			}
		}
		stage ('Deploy practica'){
			steps {
				sh '''
					cd Practica1-201403841_SA
					npm start
                '''
			}
		}
	}
}