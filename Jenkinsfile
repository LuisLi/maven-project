pipeline {
   def mvnHome
   agent any
   stages {
	stage('Build') {
		steps {
			mvnHome = tool 'M3'
			
			sh "'${mvnHome}/bin/mvn' clean package"
		}
	}
   }
}
