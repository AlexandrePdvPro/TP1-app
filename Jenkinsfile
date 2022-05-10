pipeline {

    agent {
        docker { image 'node' }
    }

    stages {

        stage('Install') {
            steps {
                sh 'node --version'
            }
        }

        stage('Build') {

            steps {

                echo 'Building..'
            }

        }

        stage('Test') {

            steps {

                echo 'Testing..'

            }

        }

        stage('Deploy') {

            steps {

                echo 'Deploying....'

            }

        }

    }

}
