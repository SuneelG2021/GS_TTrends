pipeline {
    agent {
        node {
            label 'Maven-agent'
        }
    }

    environment {
        PATH = "/usr/share/maven:$PATH"
    }

    stages {
        stage('build') {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}
