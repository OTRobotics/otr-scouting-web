pipeline {
    agent any
    stages {
        stage('Upload HTML') {
            steps {
                sh 'gsutil cp -r web gs://staging.otr-scouting.appspot.com'
            }
        }
    }
}