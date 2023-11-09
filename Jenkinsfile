pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Hello World'
               sh 'mvn install'
            }
        }
    

        stage('Dockerimage') {
            steps {
                echo 'Hello World234'
                sh 'docker build -t rsvadivu/spring-website:v2 .'
            }
        }

           stage('Dockerimage push') {
            steps {
                echo 'Image push'
                sh 'docker push rsvadivu/spring-website:v2'
            }
        }

    }
}