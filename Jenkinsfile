node {
  stage('test'){
    git 'https://github.com/Times-Now/Maven/'
  }
  stage('compile'){
    def mvnHome = tool name: 'maven-3.6.1', type: 'maven'
    sh 'mvn compile'
  }
}
  
