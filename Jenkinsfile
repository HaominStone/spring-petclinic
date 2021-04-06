pipeline {
    agent any
    tools {
        jdk 'jdk8'
    }

    stages {
        stage('build') {
            steps {
                sh '''
                    cd spring-petclinic
                    ./mvnw package'
                    java -jar target/*.jar
                    '''
            }
        }
    }
}