pipeline {
    agent any
    stages {
        stage('Upload HTML') {
            steps {
                sh "# The next line updates PATH for the Google Cloud SDK.
                    if [ -f '/var/jenkins_home/google-cloud-sdk/path.bash.inc' ]; then . '/var/jenkins_home/google-cloud-sdk/path.bash.inc';
                     fi

                    # The next line enables shell command completion for gcloud.
                    if [ -f '/var/jenkins_home/google-cloud-sdk/completion.bash.inc' ]; then . '/var/jenkins_home/google-cloud-sdk/completio
                    n.bash.inc'; fi"
                sh 'gsutil cp -r web gs://staging.otr-scouting.appspot.com'
            }
        }
    }
}