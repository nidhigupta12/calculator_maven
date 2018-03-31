pipeline {
     agent any
     stages {
          stage("Compile") {
               steps {
                    bat "mvnw compile"
               }
          }
          stage("Unit test") {
               steps {
                    bat "mvnw test"
               }
          }
		   stage("Code coverage") {
     steps {
          bat "mvnw jacocoTestReport"
          bat "mvnw jacocoTestCoverageVerification"
     }
}
		  
stage("Package") {
     steps {
          bat "mvnw package"
     }
}


	 
}
}