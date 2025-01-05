Pipeline {
    agent any

    stages {
        stage('Git checkout') {
            steps {
                echo 'This is git checkout stage'
            }
        }
        stage('build stage') {
            steps {
                echo 'This is build stage'
            }
        }
        stage('push to artifactory') {
            steps {
                echo 'This is push stage'
            }
        }
        stage('deploy') {
            steps {
                echo 'This is deploy stage'
            }
        }
    }
}
