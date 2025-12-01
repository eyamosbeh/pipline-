pipeline {
    agent any
    tools { 
        jdk 'java'      // correspond au JDK configuré
        maven 'maven'   // correspond au Maven configuré
    }
    stages {
        stage('GIT') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/eyamosbeh/pipline-.git'
            }
        }
        stage('Compile Stage') {
            steps {
                bat 'mvn clean compile'   // pour Windows
            }
        }
    }
}
