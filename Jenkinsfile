node {
  stage('SCM Checkout') {
    git 'https://github.com/harishanumandla817/dev.git'
    stage('Compile-Package') {
      def mvnHome = tool name: 'Apache Maven 3.3.9', type: 'maven'
      bat "${mvnHome}/bin/mnv package"
    }
  }
}
