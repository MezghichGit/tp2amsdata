pipeline {
   
    agent any
   
    stages {

        stage('get code from github + web hook') {
            steps {
                echo 'Pulling...';
                git branch: 'master',
                url : 'https://github.com/MezghichGit/tp2amsdata.git';
            }

            post {
                success {
                    echo "====++++success++++===="
                }
               
                failure {
                    echo "====++++failed++++===="
                }
            }
           
        }
           
    }
}