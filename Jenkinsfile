pipeline {
    agent any
    stages {
        stage('clone fron git') {
            steps {
                sh "git clone https://github.com/gdhodi/sample_code.git"
                sh "mvn clean -f sample_code"
            }
        }
        stage('test') {
            steps {
                sh "mvn test -f sample_code"
            }
        }
        stage('package') {
            steps {
                sh "mvn package -f sample_code"
            }
        }
    }
}
