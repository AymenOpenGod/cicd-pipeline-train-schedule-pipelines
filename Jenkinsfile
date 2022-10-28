pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Runing built automation'
                sh './gradlew built --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
