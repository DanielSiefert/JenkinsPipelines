pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-west-2',credentials:'aws-JenkinsPipelines') {
                    s3Upload(file:'index.html', bucket:'udacity-cloud-devops-engineer-jenkins-project', path:'index.html')
                   }
             }
        }
    }
}
