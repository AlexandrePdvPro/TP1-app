pipeline {

    agent {
        docker { image 'node:16-alpine3.14' }
    }

    stages {

        stage('Test') {
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
