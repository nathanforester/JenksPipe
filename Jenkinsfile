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
                    curl ifconfig.me
                   '''
            }
        }
    }
}
