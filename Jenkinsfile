pipeline {
    agent any
    stages {
        stage("Pull du projet") {
            steps {
                git branch: 'master', url: 'https://github.com/Kamsu500/fastapi-jenkins.git'
            }
        }
        stage("Exécution de l'image") {
            steps {
                script {
                    sh 'docker compose up -d'
                }
            }
        }
    }
}
