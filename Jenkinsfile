pipeline {
    agent any  // Runs on any available Jenkins agent

    stages {
        stage('Build WAR with Gradle') {
            steps {
                withMaven(gradle : 'Gradle-4.4.1'){
                    sh 'gradle clean build'  // Executes the Gradle build
                }
            }
        }
    }

     post {
            success {
                echo '✅ Build and deployment successful! Access app at: http://your-server-ip:8080/loginapp'
            }
            failure {
                echo '❌ Build failed! Check logs.'
            }
        }
    }
