  node{
   stage('SCM Checkout'){
     git 'https://github.com/sivaom/my-app-1'
   }
   stage('Compile-Package'){
    
      def mvnHome =  tool name: 'Maven-3.6.1', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
   }


