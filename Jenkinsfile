pipeline {
    agent any


    stages {
        stage('build') {
            steps {
                sh '''
                    pwd
                    ls
                    ./mvnw package
                    '''
            }
        }
        stage('deploy') {
            steps {
                sh '''
                    java -jar target/*.jar --server.port=8081
                '''
            }
        }
    }
}