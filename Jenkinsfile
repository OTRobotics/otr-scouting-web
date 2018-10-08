pipeline {
    agent any
    stages {
        stage('Upload HTML') {
            steps {
                sh "if [ -f '/var/jenkins_home/google-cloud-sdk/path.bash.inc' ]; then . '/var/jenkins_home/google-cloud-sdk/path.bash.inc'; fi"

                sh "if [ -f '/var/jenkins_home/google-cloud-sdk/completion.bash.inc' ]; then . '/var/jenkins_home/google-cloud-sdk/completion.bash.inc'; fi"
                sh 'gsutil cp -r web gs://staging.otr-scouting.appspot.com'
            }
        }
    }
}