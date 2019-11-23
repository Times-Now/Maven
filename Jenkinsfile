node {
  stage('SCM Checkout'){
    git 'https://github.com/Times-Now/Maven/'
  }
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven-3.6.1', type: 'maven'
    sh  "${mvnHome}/bin/mvn package"
  }
}
  
