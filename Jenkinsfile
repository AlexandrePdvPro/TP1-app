pipeline {

    agent {
        docker { image 'node:16.13.1-alpine' }
    }

    stages {

        stage('Install') {
            steps {
                echo 'Installing...'
                sh 'npm install'
            }
        }

        stage('Build') {

            steps {

                echo 'Building..'
                sh 'npm run build'
            }

        }

        stage('Test') {

            steps {

                echo 'Testing..'
                sh 'npm run test:e2e'

            }

        }

        stage('Deploy') {

            steps {

                echo 'Deploying....'
                sh 'npm run start:prod'

            }

        }

    }

}
