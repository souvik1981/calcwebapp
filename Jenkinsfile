node {

  try {
  
  stage('Code Checkout') { 
      // Get some code from a GitHub repository
      git 'https://github.com/sadanandrudraiah/calcwebapp.git'

   }
   
   stage('Unit Test') { 
      // Get some code from a GitHub repository
      bat("mvn test")

   }

} catch(e) {
	echo "Caught some exception"
}  finally {
	echo "Finally Block"
}
    
}
