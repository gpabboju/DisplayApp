node('master') {
  // stage('checkout'){
  //      git credentialsId: 'git_credentials', url: 'git@github.com:gpabboju/DisplayApp.git'
  //  }
   stage('build'){
       sh 'mvn clean package -f pom.xml'
     }
   stage('Deploy to Nexus'){
      sh 'mvn deploy'
    }
}

