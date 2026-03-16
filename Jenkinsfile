pipeline {
    agent {
        node {
            label 'Maven-agent'
        }
    }

    environment {
        PATH = "/opt/apache-maven-3.9.14/bin:$PATH"
    }

    stages {
        stage('build') {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}