pipeline {
    agent { docker 'php' }
    stages {
    	stage('test') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                	echo "Multiline shell steps works too"
                	ls -lah
                '''	
            }
        }
        stage('build') {
            steps {
                sh 'php --version'
            }
        }
    }
}