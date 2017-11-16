pipeline {
   agent any
   	stage('build'){
			steps {
				sh 'mvn build' 
			}
		}

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
