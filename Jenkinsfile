pipeline {
    agent {
        label 'docker'
    }
    options {
        sendSplunkConsoleLog()
    }
    stages {
        stage('build_project') {
            steps {
                withGradle {
                    sh './gradlew clean build'
                }
            }
        }
    }
}