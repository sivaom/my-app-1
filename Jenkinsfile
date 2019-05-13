  node{
   stage('SCM Checkout'){
     git 'https://github.com/sivaom/my-app-1'
   }
   stage('Compile-Package'){
     tool name: 'JAVA_HOME', type: 'jdk'
      def mvnHome =  tool name: 'Maven-3.6.1', type: 'maven'   
      bat "${mvnHome}/bin/mvn package"
   }
  }


