pipeline{
    agent any
    stages {
        stage('init'){
            steps {
                sh 'terraform init'
            }
        }
        stage('format') {
            steps {
                sh 'terraform fmt'
            } 
        }
        stage('validate'){
            steps {
                sh 'terraform validate'
            }
        }
        stage('validate'){
            steps {
                sh 'terraform validate'
            }
        }    
        stage('destroy'){
            steps {
                sh 'destroy --auto-approve'
            }
        }
    }
}
