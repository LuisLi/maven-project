node {
   def mvnHome
   stage('Preparation') { // for display purposes
      // Get the Maven tool.
      // ** NOTE: This 'M3' Maven tool must be configured
      // **       in the global configuration.           
      mvnHome = tool 'M3'
	  docker = tool 'MyDocker'
   }
   stage('Build') {
      sh "'${mvnHome}/bin/mvn' clean package"
	  sh "docker info"
   }
}