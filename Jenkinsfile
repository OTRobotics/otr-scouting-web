pipeline {
    agent any
    stages {
        stage('Upload HTML') {
            steps {
                sh '/var/jenkins_home/google-cloud-sdk/bin/gsutil cp -r web gs://staging.otr-scouting.appspot.com'
            }
        }
    }
}