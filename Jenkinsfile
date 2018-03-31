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
          sh "./mvnw jacocoTestReport"
          sh "./mvnw jacocoTestCoverageVerification"
     }
}
		  
stage("Package") {
     steps {
          sh "./mvnw package"
     }
}


	 
}
}