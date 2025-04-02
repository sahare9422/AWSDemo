pipeline {
    agent any
    tools {
        gradle 'gradle-8.5'  // Matches the name in Global Tools
    }
    stages {
        stage('Test Gradle') {
            steps {
                sh 'gradle -v'  // Should print Gradle 8.5
            }
        }
    }
}
