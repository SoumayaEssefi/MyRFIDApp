pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Ajoute ici les étapes de ton build (comme compiler, tester, etc.)
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Ajoute ici tes tests (par exemple make test ou autre)
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Ajoute ici tes étapes de déploiement
            }
        }
    }

    post {
        success {
            mail to: 'soumayaessefi1@gmail.com', subject: 'Build Success', body: 'Your build was successful!'
        }
        failure {
            mail to: 'soumayaessefi1@gmail.com', subject: 'Build Failed', body: 'Your build has failed.'
        }
    }
}
