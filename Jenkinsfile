node {

  try {
  
  stage('Code Checkout') { 
      // Get some code from a GitHub repository
      git 'https://github.com/rchidana/calcwebapp.git'

   }
   
   stage('Unit Test') { 
      // Get some code from a GitHub repository
      bat("mvn test")

   }
   
   stage('Test Results') {
      junit '**/target/surefire-reports/TEST-*.xml'
      archive 'target/*.jar'
   }

} catch(e) {
	echo "Caught some exception"
}  finally {
	echo "Finally Block"
}
    
}
