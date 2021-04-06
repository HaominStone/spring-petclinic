pipeline {
    agent any


    stages {
        stage('build') {
            steps {
                sh '''
                    pwd
                    ls
                    ./mvnw package
                    java -jar target/*.jar
                    '''
            }
        }
    }
}