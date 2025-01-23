pipeline {
    agent any  
    stages {
          stage("code clone") {
             steps {
                 git branch: 'main', url: 'https://github.com/Montridu/appdocker.git', credentialsId: 'github-token'
                 echo "Code cloned successfully"
             }
         }
         stage('Run Docker Command') {
            steps {
                sh 'docker ps'
            }
        }
        stage('Init'){
            steps {
                echo 'Init'
                echo '**********************************'
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
