pipeline {
    agent { 
        label 'built-in'
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