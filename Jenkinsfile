pipeline {
    agent any
    parameters {
        booleanParam(name: 'Refresh',
                    defaultValue: false,
                    description: 'Read Jenkinsfile and exit.')
		    }
    stages {
        stage('Create File') {
            steps {
                sh '''
                    sudo touch /home/jenkins/example.txt
                   '''
            }
        }
        stage('Write to File') {
            steps {
                sh '''
                    sudo echo "Hello" > /home/jenkins/example.txt
                   '''
            }
        }

        stage('Delete file') {
            steps {
                sh '''
                    sudo rm /home/jenkins/example.txt
                   '''
            }
        }
    }
}
