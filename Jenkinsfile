pipeline {
    stages {
        stage('build') {
            steps {
                sh 'cd spring-petclinic',
                sh './mvnw package',
                sh 'java -jar target/*.jar'
            }
        }
    }
}