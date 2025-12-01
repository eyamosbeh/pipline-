pipeline {
    agent any
    tools { 
        jdk 'java'
        maven 'maven'
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
                 // changer ce chemin si ton pom.xml est ailleurs
                    bat 'mvn clean compile'
                }
            }
        }
    }
}
