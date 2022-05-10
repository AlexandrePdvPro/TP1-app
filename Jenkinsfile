pipeline {

    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000 -p 5000:5000'
            args '-u 0:0'

        }
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
