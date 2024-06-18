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
                      touch /home/ubuntu/example.txt
                   '''
            }
        }
        stage('Write to File') {
            steps {
                sh '''
                      echo "Hello" > /home/ubuntu/example.txt
                   '''
            }
        }

        stage('Delete file') {
            steps {
                sh '''
                      rm /home/ubuntu/example.txt
                   '''
            }
        }
    }
}
