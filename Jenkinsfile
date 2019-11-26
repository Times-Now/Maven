ode {
   
   stage('Code checkout') { // for display purposes
     git credentialsId: 'githubID', url: 'https://github.com/Fullmavencode/maven-examples.git'  
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
  
   }
   
} 
