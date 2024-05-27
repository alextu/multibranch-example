pipeline {
    agent 'docker'
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