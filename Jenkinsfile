def NAME="PUNEET"
pipeline {
    agent {
        label 'slave1'
    }

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/spuneetkr/JLabs.git'
            }
        }
        stage('Script Execution'){
            steps {
                 sh 'chmod +x simple-script.sh'
                 sh './simple-script.sh'
                 echo "${NAME} , Hope you are well"
            }
        }
    }
}
