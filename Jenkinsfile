pipeline {
    agent any  

    stages {
          stage("code clone") {
             steps {
                 git url: "https://github.com/Montridu/appdocker.git", branch: "main"
                 echo "Code cloned successfully"
             }
         }
        stage('Init'){
            steps {
                echo 'Init'
                echo '******************************'
                docker ps
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
                echo '******************************'
            }
        }
        stage('Yarn Build image') {
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
