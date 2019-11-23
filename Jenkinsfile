node {
   
   stage('Code checkout') { // for display purposes
     git credentialsId: '1c95f2c9-ab13-4b5c-a40a-8a7c0412e4c2', url: 'https://github.com/Times-Now/Maven.git'  
   }
   stage('Build') {
    withMaven(jdk: 'JDK-1.8', maven: 'Maven-3.6.1') {
      sh 'mvn clean compile'
    } 
   }
   stage('Test') {
    withMaven(jdk: 'JDK-1.8', maven: 'Maven-3.6.1') {
      sh 'mvn test'
    }
   }
  stage('Code Analysis') {
   //withMaven(jdk: 'JDK-1.8', maven: 'Maven-3.6.1') {
   //   sh 'mvn sonar:sonar'
   // }
    
   }
   stage('Package') {
   
    withMaven(jdk: 'JDK-1.8', maven: 'Maven-3.6.1') {
      sh 'mvn package'
    }
   }
   stage('Deploy to Dev') {
   
    
   }
   
} 
