pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'eu-west-1') {
                    s3Upload(file:'index.html', bucket:'udacity-cloud-devops-engineer-jenkins-project', path:'/index.html')
                   }
             }
        }
    }
}
