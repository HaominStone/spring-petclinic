pipeline {
    agent any


    stages {
        stage('build') {
            steps {
                sh '''
                    pwd
                    ./mvnw package'
                    java -jar target/*.jar
                    '''
            }
        }
    }
}