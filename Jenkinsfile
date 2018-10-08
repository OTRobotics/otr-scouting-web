pipeline {
    agent any
    stages {
        stage('Upload HTML') {
            environment {
                GCS_CREDS = credentials('otr-scouting-web-gcloud')
            }
            steps {
                sh "/var/jenkins_home/google-cloud-sdk/bin/gcloud auth activate-service-account --key-file ${env.GCS_CREDS}"
                sh '/var/jenkins_home/google-cloud-sdk/bin/gsutil cp -r web gs://staging.otr-scouting.appspot.com'
            }
        }
    }
}