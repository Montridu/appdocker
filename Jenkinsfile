pipeline {
    
    agent any  
 
    stages {
          stage("code") {
             steps {
                 git url: "https://github.com/Montridu/appdocker.git", branch: "main"
                 echo "Code cloned successfully"
             }
         }
        stage('Init'){
            steps {
                echo 'Init'
                echo '******************************'
            }
        }
 
        stage('Yarn Install') {
            steps {
                echo 'Yarn Install'
                echo '******************************'
            }
        }
         stage('Security') {
            steps{
                echo 'Security'
                echo 'Security1'
                echo '******************************'
            }
        }
        stage('Yarn Build') {
            steps {
                echo 'Yarn Build'
                echo '******************************'
            }
        }
 

        stage('Deploy') {
            steps{
                echo 'Deploy'
                echo '******************************'
            }
        }
    }
}
