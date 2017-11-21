pipeline {
	agent any
	environment {
   		env2 = 'Nice work!'
   		env1 = 'Hello Shekhar!'
	}
	stages {
   	stage('test'){
			steps {
				sh 'mvn test' 
			}
		}

   	stage('run'){
			steps {
				sh 'mvn spring-boot:run' 
			}
		}

	}
	post {
		always {
                  start.sh
		}
		changed {
                  start1.sh
		}
	}
}
