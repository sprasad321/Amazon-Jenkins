pipeline {
    agent any
    environment {
        // Use PATH+EXTRA to append to PATH properly
        PATH = "/usr/bin:/bin:/opt/homebrew/bin"
    }
    stages {

        stage('pull scm ') {
            steps {
                git branch: 'dev', url: 'https://github.com/PraveenKuber/Amazon-Jenkins.git'
            }
        }
  post{
  success{
     echo 'Build success'
  }    
  failure{
       echo 'Failure in the build'
   }

  }


}
