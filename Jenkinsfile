pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/vanshchoudhary108/self-healing-devops-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t self-healing-app -f docker/Dockerfile .'
            }
        }

        stage('Deploy using Ansible') {
            steps {
                sh 'ansible-playbook ansible/deploy.yml'
            }
        }
    }
}
