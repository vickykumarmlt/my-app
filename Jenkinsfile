node{
  def mvnHome= tool (name: 'Apache Maven 3.6.0', type: 'maven')+'/bin/mvn'
  stage('SCM-Checkout'){
    git 'https://github.com/vickykumarmlt/my-app'
  }
  stage('Compile-package'){
    sh "${mvnHome} clean package"
  }
}
