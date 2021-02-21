pipeline {
    agent any
    tools{
        maven 'M2_HOME'
    }

    stages {
        stage('build') {
            steps {
                echo 'Hello build'
                sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
            }
        }
        stage('testy') {
            steps {
                sh 'mvn test'
            }
        }
        stage('deploy') {
            steps {
                echo 'Hello Test'
            }
        }
    }
}
