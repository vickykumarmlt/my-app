node{
  def mvnHome= tool (name: 'Apache Maven 3.6.0', type: 'maven')+'/bin/mvn'
  stage('SCM-Checkout'){
    git 'https://github.com/vickykumarmlt/my-app'
  }
  stage('Compile-package'){
    sh "${mvnHome} clean package"
  }
  stage('print 1st Time'){
    sh 'java -cp /var/lib/jenkins/workspace/my-app-pipeline/target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
  }
    stage('print 2nd Time'){
    sh 'java -cp /var/lib/jenkins/workspace/my-app-pipeline/target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
  }
   stage('echoing output from console'){
     def value=5
     sh "echo ${value} $USER $whoami"
     
  }
}
