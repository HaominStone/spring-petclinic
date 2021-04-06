pipeline {
    agent {
        node {
            label 'pet3'
        }
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