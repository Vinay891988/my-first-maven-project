pipeline {
    agent any

    stages {
        stage("Checkout") {
            steps {
                git branch: 'main', credentialsId: '', url: 'https://github.com/Vinay891988/my-first-maven-project.git'
            }
        }
        stage("Maven clean") {
            def mvnTool = tool 'Maven3'
            steps {
                sh "${mvnTool}/bin/mvn clean install"
            }
        }
    }
}      