pipeline {
     agent any
     stages {
	     
	     stage('checkout') {
          steps {
                git url: 'https://github.com/nidhigupta12/calculator_maven.git'
               
               
              
          }
        }
          stage("Compile") {
               steps {
                    sh "mvnw compile"
               }
          }
          stage("Unit test") {
               steps {
                    sh "mvnw test"
               }
          }
		   
stage("Package") {
     steps {
          sh "mvnw package"
     }
}


	 
}
}
