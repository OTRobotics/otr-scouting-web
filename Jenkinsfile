pipeline {
    agent any
    stages {
        stage('Upload HTML') {
            steps {
                bash 'gsutil cp -r web gs://staging.otr-scouting.appspot.com'
            }
        }
    }
}