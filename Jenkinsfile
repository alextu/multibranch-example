pipeline {
    agent { 
        label 'jenkins'
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