pipeline {
    agent any

    stages {
        stage("Checkout") {
            steps {
                git branch: 'main', credentialsId: '', url: 'https://github.com/Vinay891988/my-first-maven-project.git'
            }
        }
        stage("Maven clean") {
            steps {
                sh "mvn clean package"
            }
        }
    }
}      