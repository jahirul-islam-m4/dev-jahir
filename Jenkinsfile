pipeline {
	agent any

	stages {
		stage ('Compile Stage') {
			steps {
				echo 'Start Building !!'
				withMaven(maven: 'maven_3_6_0') {
					sh 'mvn clean compile'
				}
			}
		}
		stage ('Testing Stage') {
			steps {
				echo 'Start Building !!'
				withMaven(maven: 'maven_3_6_0') {
					sh 'mvn test'
				}
			}
		}
	} 
}
