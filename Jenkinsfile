pipeline {
    agent any
    stages {
        stage('Clone Code') {
            steps {
                git branch: 'main', url: 'https://github.com/your-username/static-gym-html-css-app.git'
            }
        }
        stage('Deploy Static Site') {
            steps {
                script {
                    sh 'cp -r * /var/www/static-gym-html-css-app/'
                }
            }
        }
    }
}
