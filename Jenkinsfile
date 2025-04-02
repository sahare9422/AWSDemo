pipeline {
    agent any  // Runs on any available Jenkins agent

    stages {
        stage('Checkout Git') {
            steps {
                git branch: 'master', 
                url: 'https://github.com/your-username/your-repo.git'  // Replace with your repo URL
            }
        }

        stage('Build WAR with Gradle') {
            steps {
                sh 'gradle clean build'  // Executes the Gradle build
            }
        }
    }
}
