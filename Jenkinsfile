pipeline {
    agent { label 'mvn-agent-build' }
    stages {
        stage('clone') {
            steps {
               git branch: "main", url: 'https://github.com/mounikachitiki/java-war-repo.git'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
        
    }
}
